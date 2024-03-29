# Overview Apache POI Excel
Microsoft Excel currently has 2 extensions:

- `.xls`: corresponds to Microsoft Excel 2003 and earlier versions.
This format is supported by Apache POI by java classes with the prefix `HSSF`.
- `.xlsx`: corresponds to Microsoft Excel 2007 and later versions.
This format is supported by Apache POI by java classes with the prefix `XSSF`, `SXSSF`.

# Create a maven project 
```
<dependencies>

  <!-- Excel 2003 (.xls) -->
  <!-- https://mvnrepository.com/artifact/org.apache.poi/poi -->
  <dependency>
      <groupId>org.apache.poi</groupId>
      <artifactId>poi</artifactId>
      <version>3.17</version>
  </dependency>
   
  <!-- Excel 2007 (.xlsx) -->
  <!-- https://mvnrepository.com/artifact/org.apache.poi/poi-ooxml -->
  <dependency>
      <groupId>org.apache.poi</groupId>
      <artifactId>poi-ooxml</artifactId>
      <version>3.17</version>
  </dependency>

</dependencies>
```
- Note:
  - Older version Apache POI only support file binary:  doc, xls, ppt, …
.From version 3.5, POI support more format file OOXML of MS-Office: docx, xlsx, pptx, …
  - Numeric data types when read from excel files will have a *double value*.
