---
author: KTamas
categories:
  - Export
date: 2009-03-27 12:53:36
guid: http://ktamas.blog.hu/2009/03/27/miert_fogunk_a_jovoben_excelt_is_rubyban_programozni
id: 1769356
url: /index.php/2009/03/27/miert_fogunk_a_jovoben_excelt_is_rubyban_programozni/
permalink: /index.php/2009/03/27/miert_fogunk_a_jovoben_excelt_is_rubyban_programozni/
tags: [programozás]
title: Miért fogunk a jövőben excelt is Rubyban programozni?
---

Ruby:

> require &#8216;win32ole&#8217;
  
> excel = Win32ole.new(&#8220;Excel.Application&#8221;)
  
> excel.visible = true
  
> wb = excel.workbooks.add
  
> ws = wb.activesheet
  
> ws.range(&#8216;A1:B5&#8217;).each do |cell|
  
> cell.value = &#8220;Hello, World&#8221;
  
> end

versus

> using Microsoft.Office.Interop.Excel;
  
> [&#8230;]
  
> var excel = new ApplicationClass();
  
> excel.Visible = true;
  
> object missing = System.Reflection.Missing.Value;
  
> var workbook = excel.Workbooks.Add(missing);
  
> var range = excel.get_Range((object)&#8221;A1&#8243;, (object)&#8221;B5&#8243;);
  
> foreach (Range r in range.Cells) {
  
> r.Activate();
  
> excel.ActiveCell.Value2 = &#8220;Alma&#8221;;
  
> }

Na, melik a kevésbé gány megoldás? 

(A szerkesztőségbe várjuk a jobb C#-os megoldásokat.)
