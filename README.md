# cheerio-gs
Cheerio.gs library For Google App Script or Google Spreadsheet

How to Use?
  1)First Create a App script File giving any name.
  2)Copy the Cheerio.gs code and paste on that appscript file.
  3)Save the file and create another appscript file for web scraping works.
  4)On that file you can write web scraping code using cheeerio.gs
Example and Method :
<pre>
<code>
  //link for scraping
  let link = "<a href="https://b.codewithsundeep.com">https://b.codewithsundeep.com</a>"
  //fetch the link and get content
  let fetch = UrlFetchApp.fetch(link).getContentText();
  //cheerio instance
  let cheerio = main.cgs();
  //load content in cheerio
  let $ = cheerio.load(fetch)
  Logger.log($("body").text())
</code>
</pre>
  Now You Can Use all other cheerio properties and methods following <a href="https://cheerio.js.org/">cheerio.js documentation</a>.
  
  
