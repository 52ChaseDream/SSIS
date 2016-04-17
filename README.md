<?xml version="1.0"?>
<DTS:Executable xmlns:DTS="www.microsoft.com/SqlServer/Dts"
  DTS:refId="Package"
  DTS:CreationDate="4/16/2016 5:55:18 PM"
  DTS:CreationName="Microsoft.Package"
  DTS:CreatorComputerName="DESKTOP-52MLNDA"
  DTS:CreatorName="DESKTOP-52MLNDA\Yibo Wang"
  DTS:DTSID="{64DFE130-C38A-40B7-BF8B-65781560EDBE}"
  DTS:ExecutableType="Microsoft.Package"
  DTS:LastModifiedProductVersion="13.0.1100.286"
  DTS:LocaleID="1033"
  DTS:ObjectName="Package"
  DTS:PackageType="5"
  DTS:VersionBuild="53"
  DTS:VersionGUID="{3A66696F-7172-44DE-8BF9-8864A7B75D9E}">
  <DTS:Property
    DTS:Name="PackageFormatVersion">8</DTS:Property>
  <DTS:ConnectionManagers>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataDestinationConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{65F99E66-93BA-409C-BDB6-937FB27102AE}"
      DTS:ObjectName="DataDestinationConnection">
      <DTS:PropertyExpression
        DTS:Name="ConnectionString">REPLACE( @[User::Variable] , @[User::SourceFolder] , @[User::DestinationFolder]  )</DTS:PropertyExpression>
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="lTid"
              DTS:DTSID="{4147762A-D2DE-43A4-8D6B-CB983B09A835}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="CurrencyPair"
              DTS:DTSID="{323C09B3-0569-4348-BEE9-17BD75BF6171}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateDateTime"
              DTS:DTSID="{B918F877-929E-4A1E-A6BA-AEF9B83A6EB5}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateBid"
              DTS:DTSID="{26091FD9-698F-4E0F-9CB3-0AFEA54DC6E5}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateAsk"
              DTS:DTSID="{7CAC11B2-761C-4DB1-971A-67C2C128EEAE}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="cDealable"
              DTS:DTSID="{C6EB1F69-E2D8-4238-B619-191444F39121}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="Spread"
              DTS:DTSID="{09384DD5-274A-4FE0-87C3-675E22ACA848}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:DataType="131"
              DTS:DataPrecision="30"
              DTS:DataScale="15"
              DTS:TextQualified="True"
              DTS:ObjectName="MidRate"
              DTS:DTSID="{A66F9BF8-C891-4A31-94E2-CC08E0C8FBB2}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataDestinationDailyConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{941CA524-AF18-415A-96F7-762FE0604546}"
      DTS:ObjectName="DataDestinationDailyConnection">
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252"
          DTS:ConnectionString="E:\BigData\DataDestination\DataResult\USD_JPY_Daily.csv">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="10"
              DTS:DataType="130"
              DTS:TextQualified="True"
              DTS:ObjectName="Daily"
              DTS:DTSID="{0FF7E5D2-7D3B-4FE2-9664-1BFDDD584711}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgRateBid"
              DTS:DTSID="{0A650DCD-82D8-4CC6-8BC2-C141118AA774}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgRateAsk"
              DTS:DTSID="{610CB28F-3C31-48F6-BB9E-A95718613EF7}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgMidRate"
              DTS:DTSID="{7C1741B8-DAC1-4333-BB10-86B853AAAB4F}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgSpread"
              DTS:DTSID="{70CC0D70-2A25-4AC1-9EF8-947D7EDCC9C4}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinRateBid"
              DTS:DTSID="{6AAEBD32-3178-4A2D-8351-A09FE845BA58}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinRateAsk"
              DTS:DTSID="{E7AF3DE9-E69B-4B7F-9CC6-B8C53D36D080}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinMidRate"
              DTS:DTSID="{B823964A-0990-48FA-95DD-681DBCDEC6CD}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinSpread"
              DTS:DTSID="{55494FE1-8D21-4F45-9F5D-D7D2EB812E27}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxRateBid"
              DTS:DTSID="{FFEB8951-00AA-453E-AB17-C8EF557A7B24}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxRateAsk"
              DTS:DTSID="{95B93292-0E64-4BCF-A718-E242B5425A24}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxMidRate"
              DTS:DTSID="{0BB3AD74-FC2B-4124-B093-8C61DFF81CF0}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxSpread"
              DTS:DTSID="{2C620DA7-65F4-470D-9058-4B0C83AE7D54}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataDestinationMonthlyConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{C8B01920-DF6E-4DCF-BF88-A0D3F4CCEA3D}"
      DTS:ObjectName="DataDestinationMonthlyConnection">
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:ColumnNamesInFirstDataRow="True"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252"
          DTS:ConnectionString="E:\BigData\DataDestination\DataResult\USD_JPY_Monthly.csv">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="6"
              DTS:DataType="130"
              DTS:TextQualified="True"
              DTS:ObjectName="Monthly"
              DTS:DTSID="{7C434122-09D6-4CBF-A7FD-BF23C58C4459}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgRateBid"
              DTS:DTSID="{A8B4110B-5F77-47D7-9103-4B72CB770526}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgRateAsk"
              DTS:DTSID="{B396D129-139B-45D3-92CA-9394E28CF745}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgMidRate"
              DTS:DTSID="{D71E8783-448F-48A5-AA7D-C8E03F49A74D}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgSpread"
              DTS:DTSID="{A500353F-293D-4AFF-AE76-DD90C4E9544A}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinRateBid"
              DTS:DTSID="{8DE274B7-440A-43DD-9D9F-9F63274F156A}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinRateAsk"
              DTS:DTSID="{C0BA2BD3-1849-4EAE-91E6-FCF7E0714C35}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinMidRate"
              DTS:DTSID="{DB15B3E8-C617-4500-A19B-DCD8AA25A8FF}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinSpread"
              DTS:DTSID="{728A6693-D5F6-464F-ADDA-F29F1D3E3290}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxRateBid"
              DTS:DTSID="{67199193-5390-45CF-A839-1C70C31F4697}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxRateAsk"
              DTS:DTSID="{9EA1E6DC-1AA2-4049-83BD-FFD3734907C8}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxMidRate"
              DTS:DTSID="{3C2AB377-7FB7-421E-A39E-36FAC47D22AE}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxSpread"
              DTS:DTSID="{054B7EF3-949B-40F0-95D5-E299192FABDC}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataDestinationYearlyConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{48C2912F-0C80-4E1F-9BF7-C84752C2FE5C}"
      DTS:ObjectName="DataDestinationYearlyConnection">
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:ColumnNamesInFirstDataRow="True"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252"
          DTS:ConnectionString="E:\BigData\DataDestination\DataResult\USD_JPY_Yearly.csv">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="3"
              DTS:TextQualified="True"
              DTS:ObjectName="Yearly"
              DTS:DTSID="{A947355A-21F1-4A99-92C4-6092CDBCE09C}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgRateBid"
              DTS:DTSID="{3BF6536F-5549-47CE-9011-D649288C00AA}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgRateAsk"
              DTS:DTSID="{C84FD9CF-E0AD-4030-9D36-85665BD69034}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgSpread"
              DTS:DTSID="{85FDF5D5-4BD0-4781-9A1A-26B7D8FFC550}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="AvgMidRate"
              DTS:DTSID="{8DC4EC36-3795-4AAE-B873-79598AE351B3}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinRateBid"
              DTS:DTSID="{56EBC788-B7AC-41E6-BF9B-7A86CA6F4A7E}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinRateAsk"
              DTS:DTSID="{0A0FBB13-090B-4248-BB22-14BE82D42707}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinSpread"
              DTS:DTSID="{B06B256B-B661-475E-81E5-823D04B842EF}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MinMidRate"
              DTS:DTSID="{5959E702-9F16-4806-8DC1-C60AFD5CEF85}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxRateBid"
              DTS:DTSID="{45090957-8403-424A-B8E2-1DFC6AC2FDB6}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxRateAsk"
              DTS:DTSID="{1B5ED82D-B633-4282-83C3-F3C3F4270D08}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxSpread"
              DTS:DTSID="{2499355A-D368-4042-B812-7D96A6DC5462}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="MaxMidRate"
              DTS:DTSID="{45C40FE0-D74B-49E2-9A93-440DE86B28E2}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataErrorConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{46D928DD-1DCF-46FB-A820-2B5E0D08E3FC}"
      DTS:ObjectName="DataErrorConnection">
      <DTS:PropertyExpression
        DTS:Name="ConnectionString">REPLACE( @[User::Variable] , @[User::SourceFolder] , @[User::DataErrorFolder]  )</DTS:PropertyExpression>
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="lTid"
              DTS:DTSID="{11C171A6-8FCD-472D-A9C1-312CDBB97968}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="CurrencyPair"
              DTS:DTSID="{8A46EB81-8086-426B-8ED1-92F9F3BAB32B}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateDateTime"
              DTS:DTSID="{22532986-98A1-43B8-A352-6F1C91B6A46D}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateBid"
              DTS:DTSID="{801C06CA-9ABD-4154-94E0-59F8A3462537}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateAsk"
              DTS:DTSID="{7E3DA8CD-66FF-4B77-823F-9D5BB2725756}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="cDealable"
              DTS:DTSID="{EB4B85DC-3A13-4DFE-BBE4-E5787D36F3CB}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataNullConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{4154E90F-D5B3-4DB2-8FD9-DD3A16E4277F}"
      DTS:ObjectName="DataNullConnection">
      <DTS:PropertyExpression
        DTS:Name="ConnectionString">REPLACE( @[User::Variable] , @[User::SourceFolder] , @[User::DataNULLFolder]  )</DTS:PropertyExpression>
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="lTid"
              DTS:DTSID="{0EFEAAB0-DEC4-4D2C-A17A-CC4951BE1F56}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="CurrencyPair"
              DTS:DTSID="{6E2509A1-8E00-4DCE-AF40-67D263097460}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateDateTime"
              DTS:DTSID="{0364488E-F623-4E61-BD0A-275039A6F510}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateBid"
              DTS:DTSID="{647E09E6-A3E8-4820-A2F8-A76A38813E24}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateAsk"
              DTS:DTSID="{1C4E5911-B6AB-4554-951A-66DEA04EDC73}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="cDealable"
              DTS:DTSID="{0A72E53C-0DB3-4AE8-8925-3A670FF2E0D8}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataSourceConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{52CAE292-31B7-4B83-9165-9D2DE15940B7}"
      DTS:ObjectName="DataSourceConnection">
      <DTS:PropertyExpression
        DTS:Name="ConnectionString">@[User::Variable]</DTS:PropertyExpression>
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="Column 0"
              DTS:DTSID="{91BFBFD1-1972-46FA-8551-4820D7994BD4}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="Column 1"
              DTS:DTSID="{4FD20794-A816-491C-95A2-65F284EB858B}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="Column 2"
              DTS:DTSID="{E3D17566-F659-4FA7-B992-6E130828DC1C}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="Column 3"
              DTS:DTSID="{DF3FEA4B-2C0A-411A-A7A0-26AAA98D8E71}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="Column 4"
              DTS:DTSID="{0D4301B7-1FFE-4582-A7FB-39D51F39ADF9}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="Column 5"
              DTS:DTSID="{C6A556B6-1C6A-412E-B0DD-83CAA4561558}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
    <DTS:ConnectionManager
      DTS:refId="Package.ConnectionManagers[DataTotalDestinationConnection]"
      DTS:CreationName="FLATFILE"
      DTS:DTSID="{4C5B791D-DA45-4BF9-B85F-F3E2231162C4}"
      DTS:ObjectName="DataTotalDestinationConnection">
      <DTS:ObjectData>
        <DTS:ConnectionManager
          DTS:Format="Delimited"
          DTS:LocaleID="1033"
          DTS:HeaderRowDelimiter="_x000D__x000A_"
          DTS:RowDelimiter=""
          DTS:TextQualifier="_x003C_none_x003E_"
          DTS:CodePage="1252"
          DTS:ConnectionString="E:\BigData\DataDestination\DataResult\USD_JPY_Total.csv">
          <DTS:FlatFileColumns>
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="lTid"
              DTS:DTSID="{1B0F3E91-3A84-4748-9EAC-17F89DACD58F}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="CurrencyPair"
              DTS:DTSID="{2A04B98C-649B-48C6-B6DF-B4BCD75D3BA2}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateDateTime"
              DTS:DTSID="{711AF7A4-786A-48D4-B328-EE380558DC25}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateBid"
              DTS:DTSID="{06D584E5-330A-448C-81E5-B24D578C9E36}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="RateAsk"
              DTS:DTSID="{DCC4A507-07BD-4AD5-B5EB-694357B24B50}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:MaximumWidth="50"
              DTS:DataType="129"
              DTS:TextQualified="True"
              DTS:ObjectName="cDealable"
              DTS:DTSID="{2DEB830D-BAF5-4DE7-BBDB-2C8BDC06E5CA}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x002C_"
              DTS:DataType="6"
              DTS:TextQualified="True"
              DTS:ObjectName="Spread"
              DTS:DTSID="{083E8C51-AF2F-4549-8789-864008272511}"
              DTS:CreationName="" />
            <DTS:FlatFileColumn
              DTS:ColumnType="Delimited"
              DTS:ColumnDelimiter="_x000D__x000A_"
              DTS:DataType="131"
              DTS:DataPrecision="30"
              DTS:DataScale="15"
              DTS:TextQualified="True"
              DTS:ObjectName="MidRate"
              DTS:DTSID="{E0E49B71-AC7C-4738-A28C-4F0C2C933CA0}"
              DTS:CreationName="" />
          </DTS:FlatFileColumns>
        </DTS:ConnectionManager>
      </DTS:ObjectData>
    </DTS:ConnectionManager>
  </DTS:ConnectionManagers>
  <DTS:PackageParameters>
    <DTS:PackageParameter
      DTS:CreationName=""
      DTS:DataType="8"
      DTS:DTSID="{1AAC8107-0F66-4DAD-B8ED-B4272325AD2E}"
      DTS:ObjectName="AddSplit">
      <DTS:Property
        DTS:DataType="8"
        DTS:Name="ParameterValue">" - "</DTS:Property>
    </DTS:PackageParameter>
  </DTS:PackageParameters>
  <DTS:Variables>
    <DTS:Variable
      DTS:CreationName=""
      DTS:DTSID="{5574B99E-E60A-48E2-9284-A6980339282E}"
      DTS:IncludeInDebugDump="2345"
      DTS:Namespace="User"
      DTS:ObjectName="DataErrorFolder">
      <DTS:VariableValue
        DTS:DataType="8">E:\BigData\DataDestination\DataError</DTS:VariableValue>
    </DTS:Variable>
    <DTS:Variable
      DTS:CreationName=""
      DTS:DTSID="{6E6E5810-DF64-4D37-9F58-0EA31170F20D}"
      DTS:IncludeInDebugDump="2345"
      DTS:Namespace="User"
      DTS:ObjectName="DataNULLFolder">
      <DTS:VariableValue
        DTS:DataType="8">E:\BigData\DataDestination\DataNULL</DTS:VariableValue>
    </DTS:Variable>
    <DTS:Variable
      DTS:CreationName=""
      DTS:DTSID="{1CC2F820-144F-4403-9B4E-90E60EBEBBB6}"
      DTS:IncludeInDebugDump="2345"
      DTS:Namespace="User"
      DTS:ObjectName="DestinationFolder">
      <DTS:VariableValue
        DTS:DataType="8">E:\BigData\DataDestination</DTS:VariableValue>
    </DTS:Variable>
    <DTS:Variable
      DTS:CreationName=""
      DTS:DTSID="{FDB0DCB3-F048-465F-807B-F8C8FA3CAF80}"
      DTS:IncludeInDebugDump="2345"
      DTS:Namespace="User"
      DTS:ObjectName="SourceFolder">
      <DTS:VariableValue
        DTS:DataType="8">E:\BigData\DataSource</DTS:VariableValue>
    </DTS:Variable>
    <DTS:Variable
      DTS:CreationName=""
      DTS:DTSID="{C9249720-9026-4723-83A2-BC7F1DE83D76}"
      DTS:IncludeInDebugDump="2345"
      DTS:Namespace="User"
      DTS:ObjectName="Variable">
      <DTS:VariableValue
        DTS:DataType="8"
        xml:space="preserve"></DTS:VariableValue>
    </DTS:Variable>
  </DTS:Variables>
  <DTS:Executables>
    <DTS:Executable
      DTS:refId="Package\Data Flow Task"
      DTS:CreationName="Microsoft.Pipeline"
      DTS:Description="Data Flow Task"
      DTS:DTSID="{99B9694C-8C0C-46EA-A675-125A35E3177C}"
      DTS:ExecutableType="Microsoft.Pipeline"
      DTS:LocaleID="-1"
      DTS:ObjectName="Data Flow Task"
      DTS:TaskContact="Performs high-performance data extraction, transformation and loading;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved;http://www.microsoft.com/sql/support/default.asp;1">
      <DTS:Variables />
      <DTS:ObjectData>
        <pipeline
          version="1">
          <components>
            <component
              refId="Package\Data Flow Task\Data Conversion"
              componentClassID="Microsoft.DataConvert"
              contactInfo="Data Conversion;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
              description="Data Conversion"
              name="Data Conversion"
              usesDispositions="true">
              <inputs>
                <input
                  refId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]"
                  name="Data Conversion Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[RateDateTime]"
                      cachedCodepage="1252"
                      cachedDataType="str"
                      cachedLength="50"
                      cachedName="RateDateTime"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateDateTime]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[RateBid]"
                      cachedCodepage="1252"
                      cachedDataType="str"
                      cachedLength="50"
                      cachedName="RateBid"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[RateAsk]"
                      cachedCodepage="1252"
                      cachedDataType="str"
                      cachedLength="50"
                      cachedName="RateAsk"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[MidRate]"
                      cachedDataType="numeric"
                      cachedName="MidRate"
                      cachedPrecision="30"
                      cachedScale="15"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[MidRate]" />
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output]"
                  exclusionGroup="1"
                  name="Data Conversion Output"
                  synchronousInputId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]"
                      dataType="dbTimeStamp"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]"
                      name="Copy of RateDateTime"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the input column used as the source of data for the conversion."
                          name="SourceInputColumnLineageID">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateDateTime]}</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]"
                      dataType="cy"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]"
                      name="Copy of RateBid"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the input column used as the source of data for the conversion."
                          name="SourceInputColumnLineageID">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateBid]}</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]"
                      dataType="cy"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]"
                      name="Copy of RateAsk"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the input column used as the source of data for the conversion."
                          name="SourceInputColumnLineageID">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateAsk]}</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]"
                      dataType="cy"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]"
                      name="Copy of MidRate"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the input column used as the source of data for the conversion."
                          name="SourceInputColumnLineageID">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[MidRate]}</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
                <output
                  refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output]"
                  exclusionGroup="1"
                  isErrorOut="true"
                  name="Data Conversion Error Output"
                  synchronousInputId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorCode]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorCode]"
                      name="ErrorCode"
                      specialFlags="1" />
                    <outputColumn
                      refId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorColumn]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorColumn]"
                      name="ErrorColumn"
                      specialFlags="2" />
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Data Daily"
              componentClassID="Microsoft.Aggregate"
              contactInfo="Aggregate;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;3"
              description="Aggregates data with functions such as Average, Sum, Count, Max, and Min. For example, group data to compute the sum of sales per product or the average visits per day."
              name="Data Daily"
              version="3">
              <properties>
                <property
                  dataType="System.Int32"
                  description="Specifies the approximate number of group by keys that the aggregation produces. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no KeyScale value is used."
                  name="KeyScale"
                  typeConverter="KeyScaleType">0</property>
                <property
                  dataType="System.Null"
                  description="Specifies the exact number of group by keys that the aggregation produces. If a KeyScale value is specified, the value in Keys takes precedence."
                  name="Keys" />
                <property
                  dataType="System.Int32"
                  description="Specifies the approximate number of distinct values in a column that the aggregation counts distinctly. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no CountDistinctScale value is used."
                  name="CountDistinctScale"
                  typeConverter="KeyScaleType">0</property>
                <property
                  dataType="System.Null"
                  description="Specifies the exact number of distinct values in a column that the aggregation counts distinctly. If a CountDistinctScale value is specified, the value in CountDistinctKeys takes precedence."
                  name="CountDistinctKeys" />
                <property
                  dataType="System.Int32"
                  description="Specifies the percentage by which memory can be extended during the aggregation. Valid values are between 1 and 100."
                  name="AutoExtendFactor">25</property>
              </properties>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Data Daily.Inputs[Aggregate Input 1]"
                  name="Aggregate Input 1">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Data Daily.Inputs[Aggregate Input 1].Columns[Daily]"
                      cachedDataType="wstr"
                      cachedLength="10"
                      cachedName="Daily"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Daily]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Daily.Inputs[Aggregate Input 1].Columns[Copy of RateBid]"
                      cachedDataType="cy"
                      cachedName="Copy of RateBid"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Daily.Inputs[Aggregate Input 1].Columns[Copy of RateAsk]"
                      cachedDataType="cy"
                      cachedName="Copy of RateAsk"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Daily.Inputs[Aggregate Input 1].Columns[Copy of MidRate]"
                      cachedDataType="cy"
                      cachedName="Copy of MidRate"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Daily.Inputs[Aggregate Input 1].Columns[Spread]"
                      cachedDataType="cy"
                      cachedName="Spread"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]" />
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1]"
                  name="Aggregate Output 1">
                  <properties>
                    <property
                      dataType="System.Int32"
                      description="Specifies the approximate number of group by keys that the aggregation produces. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no KeyScale value is used."
                      name="KeyScale"
                      typeConverter="KeyScaleType">0</property>
                    <property
                      dataType="System.Null"
                      description="Specifies the exact number of group by keys that the aggregation produces. If a KeyScale value is specified, the value in Keys takes precedence."
                      name="Keys" />
                  </properties>
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[Daily]"
                      dataType="wstr"
                      length="10"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[Daily]"
                      name="Daily">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Daily]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">0</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateBid]"
                      name="AvgRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateAsk]"
                      name="AvgRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgMidRate]"
                      name="AvgMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgSpread]"
                      name="AvgSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateBid]"
                      name="MinRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateAsk]"
                      name="MinRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinMidRate]"
                      name="MinMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinSpread]"
                      name="MinSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateBid]"
                      name="MaxRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateAsk]"
                      name="MaxRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxMidRate]"
                      name="MaxMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxSpread]"
                      name="MaxSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Data Destination Daily"
              componentClassID="Microsoft.FlatFileDestination"
              contactInfo="Flat File Destination;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
              description="Flat File Destination"
              localeId="1033"
              name="Data Destination Daily">
              <properties>
                <property
                  dataType="System.Boolean"
                  description="Specifies whether the data will overwrite or append to the destination file."
                  name="Overwrite">true</property>
                <property
                  dataType="System.Null"
                  description="Specifies the text to write to the destination file before any data is written."
                  expressionType="Notify"
                  name="Header" />
              </properties>
              <connections>
                <connection
                  refId="Package\Data Flow Task\Data Destination Daily.Connections[FlatFileConnection]"
                  connectionManagerID="Package.ConnectionManagers[DataDestinationDailyConnection]"
                  connectionManagerRefId="Package.ConnectionManagers[DataDestinationDailyConnection]"
                  name="FlatFileConnection" />
              </connections>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input]"
                  hasSideEffects="true"
                  name="Flat File Destination Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[AvgRateBid]"
                      cachedDataType="cy"
                      cachedName="AvgRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgRateBid]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[AvgRateAsk]"
                      cachedDataType="cy"
                      cachedName="AvgRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[AvgMidRate]"
                      cachedDataType="cy"
                      cachedName="AvgMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgMidRate]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[AvgSpread]"
                      cachedDataType="cy"
                      cachedName="AvgSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgSpread]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MinRateBid]"
                      cachedDataType="cy"
                      cachedName="MinRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinRateBid]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MinRateAsk]"
                      cachedDataType="cy"
                      cachedName="MinRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MinMidRate]"
                      cachedDataType="cy"
                      cachedName="MinMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinMidRate]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MinSpread]"
                      cachedDataType="cy"
                      cachedName="MinSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinSpread]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MaxRateBid]"
                      cachedDataType="cy"
                      cachedName="MaxRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxRateBid]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MaxRateAsk]"
                      cachedDataType="cy"
                      cachedName="MaxRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MaxMidRate]"
                      cachedDataType="cy"
                      cachedName="MaxMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxMidRate]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[MaxSpread]"
                      cachedDataType="cy"
                      cachedName="MaxSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxSpread]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].Columns[Daily]"
                      cachedDataType="wstr"
                      cachedLength="10"
                      cachedName="Daily"
                      cachedSortKeyPosition="-1"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[Daily]"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[Daily]" />
                  </inputColumns>
                  <externalMetadataColumns
                    isUsed="True">
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[Daily]"
                      dataType="wstr"
                      length="10"
                      name="Daily" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgRateBid]"
                      dataType="cy"
                      name="AvgRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgRateAsk]"
                      dataType="cy"
                      name="AvgRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgMidRate]"
                      dataType="cy"
                      name="AvgMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[AvgSpread]"
                      dataType="cy"
                      name="AvgSpread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinRateBid]"
                      dataType="cy"
                      name="MinRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinRateAsk]"
                      dataType="cy"
                      name="MinRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinMidRate]"
                      dataType="cy"
                      name="MinMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MinSpread]"
                      dataType="cy"
                      name="MinSpread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxRateBid]"
                      dataType="cy"
                      name="MaxRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxRateAsk]"
                      dataType="cy"
                      name="MaxRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxMidRate]"
                      dataType="cy"
                      name="MaxMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input].ExternalColumns[MaxSpread]"
                      dataType="cy"
                      name="MaxSpread" />
                  </externalMetadataColumns>
                </input>
              </inputs>
            </component>
            <component
              refId="Package\Data Flow Task\Data Destination Monthly"
              componentClassID="Microsoft.FlatFileDestination"
              contactInfo="Flat File Destination;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
              description="Flat File Destination"
              localeId="1033"
              name="Data Destination Monthly">
              <properties>
                <property
                  dataType="System.Boolean"
                  description="Specifies whether the data will overwrite or append to the destination file."
                  name="Overwrite">true</property>
                <property
                  dataType="System.Null"
                  description="Specifies the text to write to the destination file before any data is written."
                  expressionType="Notify"
                  name="Header" />
              </properties>
              <connections>
                <connection
                  refId="Package\Data Flow Task\Data Destination Monthly.Connections[FlatFileConnection]"
                  connectionManagerID="Package.ConnectionManagers[DataDestinationMonthlyConnection]"
                  connectionManagerRefId="Package.ConnectionManagers[DataDestinationMonthlyConnection]"
                  name="FlatFileConnection" />
              </connections>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input]"
                  hasSideEffects="true"
                  name="Flat File Destination Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[Monthly]"
                      cachedDataType="wstr"
                      cachedLength="7"
                      cachedName="Monthly"
                      cachedSortKeyPosition="-1"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[Monthly]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[Monthly]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[AvgRateBid]"
                      cachedDataType="cy"
                      cachedName="AvgRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateBid]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[AvgRateAsk]"
                      cachedDataType="cy"
                      cachedName="AvgRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[AvgMidRate]"
                      cachedDataType="cy"
                      cachedName="AvgMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgMidRate]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[AvgSpread]"
                      cachedDataType="cy"
                      cachedName="AvgSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgSpread]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MinRateBid]"
                      cachedDataType="cy"
                      cachedName="MinRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinRateBid]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MinRateAsk]"
                      cachedDataType="cy"
                      cachedName="MinRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MinMidRate]"
                      cachedDataType="cy"
                      cachedName="MinMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinMidRate]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MinSpread]"
                      cachedDataType="cy"
                      cachedName="MinSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinSpread]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MaxRateBid]"
                      cachedDataType="cy"
                      cachedName="MaxRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateBid]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MaxRateAsk]"
                      cachedDataType="cy"
                      cachedName="MaxRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MaxMidRate]"
                      cachedDataType="cy"
                      cachedName="MaxMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxMidRate]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].Columns[MaxSpread]"
                      cachedDataType="cy"
                      cachedName="MaxSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxSpread]"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxSpread]" />
                  </inputColumns>
                  <externalMetadataColumns
                    isUsed="True">
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[Monthly]"
                      dataType="wstr"
                      length="6"
                      name="Monthly" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateBid]"
                      dataType="cy"
                      name="AvgRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateAsk]"
                      dataType="cy"
                      name="AvgRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgMidRate]"
                      dataType="cy"
                      name="AvgMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[AvgSpread]"
                      dataType="cy"
                      name="AvgSpread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinRateBid]"
                      dataType="cy"
                      name="MinRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinRateAsk]"
                      dataType="cy"
                      name="MinRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinMidRate]"
                      dataType="cy"
                      name="MinMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MinSpread]"
                      dataType="cy"
                      name="MinSpread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateBid]"
                      dataType="cy"
                      name="MaxRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateAsk]"
                      dataType="cy"
                      name="MaxRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxMidRate]"
                      dataType="cy"
                      name="MaxMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input].ExternalColumns[MaxSpread]"
                      dataType="cy"
                      name="MaxSpread" />
                  </externalMetadataColumns>
                </input>
              </inputs>
            </component>
            <component
              refId="Package\Data Flow Task\Data Destination Yearly"
              componentClassID="Microsoft.FlatFileDestination"
              contactInfo="Flat File Destination;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
              description="Flat File Destination"
              localeId="1033"
              name="Data Destination Yearly">
              <properties>
                <property
                  dataType="System.Boolean"
                  description="Specifies whether the data will overwrite or append to the destination file."
                  name="Overwrite">true</property>
                <property
                  dataType="System.Null"
                  description="Specifies the text to write to the destination file before any data is written."
                  expressionType="Notify"
                  name="Header" />
              </properties>
              <connections>
                <connection
                  refId="Package\Data Flow Task\Data Destination Yearly.Connections[FlatFileConnection]"
                  connectionManagerID="Package.ConnectionManagers[DataDestinationYearlyConnection]"
                  connectionManagerRefId="Package.ConnectionManagers[DataDestinationYearlyConnection]"
                  name="FlatFileConnection" />
              </connections>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input]"
                  hasSideEffects="true"
                  name="Flat File Destination Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[Yearly]"
                      cachedDataType="i4"
                      cachedName="Yearly"
                      cachedSortKeyPosition="-1"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[Yearly]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[Yearly]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[AvgRateBid]"
                      cachedDataType="cy"
                      cachedName="AvgRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateBid]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[AvgRateAsk]"
                      cachedDataType="cy"
                      cachedName="AvgRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MinRateBid]"
                      cachedDataType="cy"
                      cachedName="MinRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinRateBid]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MaxRateBid]"
                      cachedDataType="cy"
                      cachedName="MaxRateBid"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateBid]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxRateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[AvgSpread]"
                      cachedDataType="cy"
                      cachedName="AvgSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgSpread]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[AvgMidRate]"
                      cachedDataType="cy"
                      cachedName="AvgMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgMidRate]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MinSpread]"
                      cachedDataType="cy"
                      cachedName="MinSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinSpread]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MinMidRate]"
                      cachedDataType="cy"
                      cachedName="MinMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinMidRate]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MaxSpread]"
                      cachedDataType="cy"
                      cachedName="MaxSpread"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxSpread]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxSpread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MaxMidRate]"
                      cachedDataType="cy"
                      cachedName="MaxMidRate"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxMidRate]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxMidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MinRateAsk]"
                      cachedDataType="cy"
                      cachedName="MinRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinRateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].Columns[MaxRateAsk]"
                      cachedDataType="cy"
                      cachedName="MaxRateAsk"
                      externalMetadataColumnId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateAsk]"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxRateAsk]" />
                  </inputColumns>
                  <externalMetadataColumns
                    isUsed="True">
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[Yearly]"
                      dataType="i4"
                      name="Yearly" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateBid]"
                      dataType="cy"
                      name="AvgRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgRateAsk]"
                      dataType="cy"
                      name="AvgRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinRateBid]"
                      dataType="cy"
                      name="MinRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateBid]"
                      dataType="cy"
                      name="MaxRateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxRateAsk]"
                      dataType="cy"
                      name="MaxRateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgSpread]"
                      dataType="cy"
                      name="AvgSpread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[AvgMidRate]"
                      dataType="cy"
                      name="AvgMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinSpread]"
                      dataType="cy"
                      name="MinSpread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinMidRate]"
                      dataType="cy"
                      name="MinMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxSpread]"
                      dataType="cy"
                      name="MaxSpread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MaxMidRate]"
                      dataType="cy"
                      name="MaxMidRate" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input].ExternalColumns[MinRateAsk]"
                      dataType="cy"
                      name="MinRateAsk" />
                  </externalMetadataColumns>
                </input>
              </inputs>
            </component>
            <component
              refId="Package\Data Flow Task\Data Monthly"
              componentClassID="Microsoft.Aggregate"
              contactInfo="Aggregate;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;3"
              description="Aggregates data with functions such as Average, Sum, Count, Max, and Min. For example, group data to compute the sum of sales per product or the average visits per day."
              name="Data Monthly"
              version="3">
              <properties>
                <property
                  dataType="System.Int32"
                  description="Specifies the approximate number of group by keys that the aggregation produces. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no KeyScale value is used."
                  name="KeyScale"
                  typeConverter="KeyScaleType">0</property>
                <property
                  dataType="System.Null"
                  description="Specifies the exact number of group by keys that the aggregation produces. If a KeyScale value is specified, the value in Keys takes precedence."
                  name="Keys" />
                <property
                  dataType="System.Int32"
                  description="Specifies the approximate number of distinct values in a column that the aggregation counts distinctly. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no CountDistinctScale value is used."
                  name="CountDistinctScale"
                  typeConverter="KeyScaleType">0</property>
                <property
                  dataType="System.Null"
                  description="Specifies the exact number of distinct values in a column that the aggregation counts distinctly. If a CountDistinctScale value is specified, the value in CountDistinctKeys takes precedence."
                  name="CountDistinctKeys" />
                <property
                  dataType="System.Int32"
                  description="Specifies the percentage by which memory can be extended during the aggregation. Valid values are between 1 and 100."
                  name="AutoExtendFactor">25</property>
              </properties>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Data Monthly.Inputs[Aggregate Input 1]"
                  name="Aggregate Input 1">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Data Monthly.Inputs[Aggregate Input 1].Columns[Monthly]"
                      cachedDataType="wstr"
                      cachedLength="7"
                      cachedName="Monthly"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Monthly]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Monthly.Inputs[Aggregate Input 1].Columns[Copy of RateBid]"
                      cachedDataType="cy"
                      cachedName="Copy of RateBid"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Monthly.Inputs[Aggregate Input 1].Columns[Copy of RateAsk]"
                      cachedDataType="cy"
                      cachedName="Copy of RateAsk"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Monthly.Inputs[Aggregate Input 1].Columns[Copy of MidRate]"
                      cachedDataType="cy"
                      cachedName="Copy of MidRate"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Monthly.Inputs[Aggregate Input 1].Columns[Spread]"
                      cachedDataType="cy"
                      cachedName="Spread"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]" />
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1]"
                  name="Aggregate Output 1">
                  <properties>
                    <property
                      dataType="System.Int32"
                      description="Specifies the approximate number of group by keys that the aggregation produces. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no KeyScale value is used."
                      name="KeyScale"
                      typeConverter="KeyScaleType">0</property>
                    <property
                      dataType="System.Null"
                      description="Specifies the exact number of group by keys that the aggregation produces. If a KeyScale value is specified, the value in Keys takes precedence."
                      name="Keys" />
                  </properties>
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[Monthly]"
                      dataType="wstr"
                      length="7"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[Monthly]"
                      name="Monthly">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Monthly]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">0</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateBid]"
                      name="AvgRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]"
                      name="AvgRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgMidRate]"
                      name="AvgMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgSpread]"
                      name="AvgSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateBid]"
                      name="MinRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateAsk]"
                      name="MinRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinMidRate]"
                      name="MinMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinSpread]"
                      name="MinSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateBid]"
                      name="MaxRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]"
                      name="MaxRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxMidRate]"
                      name="MaxMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxSpread]"
                      name="MaxSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Data Yearly"
              componentClassID="Microsoft.Aggregate"
              contactInfo="Aggregate;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;3"
              description="Aggregates data with functions such as Average, Sum, Count, Max, and Min. For example, group data to compute the sum of sales per product or the average visits per day."
              name="Data Yearly"
              version="3">
              <properties>
                <property
                  dataType="System.Int32"
                  description="Specifies the approximate number of group by keys that the aggregation produces. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no KeyScale value is used."
                  name="KeyScale"
                  typeConverter="KeyScaleType">0</property>
                <property
                  dataType="System.Null"
                  description="Specifies the exact number of group by keys that the aggregation produces. If a KeyScale value is specified, the value in Keys takes precedence."
                  name="Keys" />
                <property
                  dataType="System.Int32"
                  description="Specifies the approximate number of distinct values in a column that the aggregation counts distinctly. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no CountDistinctScale value is used."
                  name="CountDistinctScale"
                  typeConverter="KeyScaleType">0</property>
                <property
                  dataType="System.Null"
                  description="Specifies the exact number of distinct values in a column that the aggregation counts distinctly. If a CountDistinctScale value is specified, the value in CountDistinctKeys takes precedence."
                  name="CountDistinctKeys" />
                <property
                  dataType="System.Int32"
                  description="Specifies the percentage by which memory can be extended during the aggregation. Valid values are between 1 and 100."
                  name="AutoExtendFactor">25</property>
              </properties>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Data Yearly.Inputs[Aggregate Input 1]"
                  name="Aggregate Input 1">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Data Yearly.Inputs[Aggregate Input 1].Columns[Yearly]"
                      cachedDataType="i4"
                      cachedName="Yearly"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Yearly]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Yearly.Inputs[Aggregate Input 1].Columns[Copy of RateBid]"
                      cachedDataType="cy"
                      cachedName="Copy of RateBid"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Yearly.Inputs[Aggregate Input 1].Columns[Copy of RateAsk]"
                      cachedDataType="cy"
                      cachedName="Copy of RateAsk"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Yearly.Inputs[Aggregate Input 1].Columns[Spread]"
                      cachedDataType="cy"
                      cachedName="Spread"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]" />
                    <inputColumn
                      refId="Package\Data Flow Task\Data Yearly.Inputs[Aggregate Input 1].Columns[Copy of MidRate]"
                      cachedDataType="cy"
                      cachedName="Copy of MidRate"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]" />
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1]"
                  name="Aggregate Output 1">
                  <properties>
                    <property
                      dataType="System.Int32"
                      description="Specifies the approximate number of group by keys that the aggregation produces. Low indicates 500,000 key values, Medium indicates 5 million key values, and High indicates more than 25 million key values. Unspecified indicates no KeyScale value is used."
                      name="KeyScale"
                      typeConverter="KeyScaleType">0</property>
                    <property
                      dataType="System.Null"
                      description="Specifies the exact number of group by keys that the aggregation produces. If a KeyScale value is specified, the value in Keys takes precedence."
                      name="Keys" />
                  </properties>
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[Yearly]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[Yearly]"
                      name="Yearly">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Yearly]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">0</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateBid]"
                      name="AvgRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]"
                      name="AvgRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgSpread]"
                      name="AvgSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgMidRate]"
                      name="AvgMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">5</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateBid]"
                      name="MinRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateAsk]"
                      name="MinRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinSpread]"
                      name="MinSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinMidRate]"
                      name="MinMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">6</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateBid]"
                      name="MaxRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]"
                      name="MaxRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxSpread]"
                      name="MaxSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxMidRate]"
                      name="MaxMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the ID of the input column used in the aggregation."
                          name="AggregationColumnId">#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of MidRate]}</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the type of aggregation."
                          name="AggregationType"
                          typeConverter="AggregationType">7</property>
                        <property
                          dataType="System.Int32"
                          description="Indicates whether the column requires special handling because it may contain oversized data or it requires precision beyond a float data type."
                          name="IsBig">1</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the string comparison options."
                          name="AggregationComparisonFlags">0</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Derived Column"
              componentClassID="Microsoft.DerivedColumn"
              contactInfo="Derived Column;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
              description="Creates new column values by applying expressions to transformation input columns. Create new columns or overwrite existing ones. For example, concatenate the values from the 'first name' and 'last name' column to make a 'full name' column."
              name="Derived Column"
              usesDispositions="true">
              <inputs>
                <input
                  refId="Package\Data Flow Task\Derived Column.Inputs[Derived Column Input]"
                  description="Input to the Derived Column Transformation"
                  name="Derived Column Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Derived Column.Inputs[Derived Column Input].Columns[Copy of RateDateTime]"
                      cachedDataType="dbTimeStamp"
                      cachedName="Copy of RateDateTime"
                      lineageId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]" />
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output]"
                  description="Default Output of the Derived Column Transformation"
                  exclusionGroup="1"
                  name="Derived Column Output"
                  synchronousInputId="Package\Data Flow Task\Derived Column.Inputs[Derived Column Input]">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Yearly]"
                      dataType="i4"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Yearly]"
                      name="Yearly"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Derived Column Expression"
                          name="Expression">[YEAR](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]})</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Derived Column Friendly Expression"
                          expressionType="Notify"
                          name="FriendlyExpression">YEAR([Copy of RateDateTime])</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Monthly]"
                      dataType="wstr"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      length="7"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Monthly]"
                      name="Monthly"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Derived Column Expression"
                          name="Expression">(DT_STR,4,1252)[YEAR](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) + "-" + ([MONTH](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) &lt; 10 ? "0" + (DT_STR,1,1252)[MONTH](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) : (DT_STR,2,1252)[MONTH](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}))</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Derived Column Friendly Expression"
                          expressionType="Notify"
                          name="FriendlyExpression">(DT_STR,4,1252)YEAR([Copy of RateDateTime]) + "-" + (MONTH([Copy of RateDateTime]) &lt; 10 ? "0" + (DT_STR,1,1252)MONTH([Copy of RateDateTime]) : (DT_STR,2,1252)MONTH([Copy of RateDateTime]))</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Daily]"
                      dataType="wstr"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      length="10"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Daily]"
                      name="Daily"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Derived Column Expression"
                          name="Expression">(DT_STR,4,1252)[YEAR](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) + "-" + ([MONTH](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) &lt; 10 ? "0" + (DT_STR,1,1252)[MONTH](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) : (DT_STR,2,1252)[MONTH](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]})) + "-" + ([DAY](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) &lt; 10 ? "0" + (DT_STR,1,1252)[DAY](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}) : (DT_STR,2,1252)[DAY](#{Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]}))</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Derived Column Friendly Expression"
                          expressionType="Notify"
                          name="FriendlyExpression">(DT_STR,4,1252)YEAR([Copy of RateDateTime]) + "-" + (MONTH([Copy of RateDateTime]) &lt; 10 ? "0" + (DT_STR,1,1252)MONTH([Copy of RateDateTime]) : (DT_STR,2,1252)MONTH([Copy of RateDateTime])) + "-" + (DAY([Copy of RateDateTime]) &lt; 10 ? "0" + (DT_STR,1,1252)DAY([Copy of RateDateTime]) : (DT_STR,2,1252)DAY([Copy of RateDateTime]))</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
                <output
                  refId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Error Output]"
                  description="Error Output of the Derived Column Transformation"
                  exclusionGroup="1"
                  isErrorOut="true"
                  name="Derived Column Error Output"
                  synchronousInputId="Package\Data Flow Task\Derived Column.Inputs[Derived Column Input]">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorCode]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorCode]"
                      name="ErrorCode"
                      specialFlags="1" />
                    <outputColumn
                      refId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorColumn]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorColumn]"
                      name="ErrorColumn"
                      specialFlags="2" />
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Flat File Source"
              componentClassID="Microsoft.FlatFileSource"
              contactInfo="Flat File Source;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;1"
              description="Flat File Source"
              localeId="1033"
              name="Flat File Source"
              usesDispositions="true"
              version="1">
              <properties>
                <property
                  dataType="System.Boolean"
                  description="Specifies whether zero-length columns are treated as null."
                  name="RetainNulls">false</property>
                <property
                  dataType="System.String"
                  description="Specifies the name of an output column containing the file name. If no name is specified, no output column containing the file name will be generated."
                  name="FileNameColumnName"></property>
              </properties>
              <connections>
                <connection
                  refId="Package\Data Flow Task\Flat File Source.Connections[FlatFileConnection]"
                  connectionManagerID="Package.ConnectionManagers[DataTotalDestinationConnection]"
                  connectionManagerRefId="Package.ConnectionManagers[DataTotalDestinationConnection]"
                  name="FlatFileConnection" />
              </connections>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output]"
                  name="Flat File Source Output">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[lTid]"
                      codePage="1252"
                      dataType="str"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[lTid]"
                      length="50"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[lTid]"
                      name="lTid"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[CurrencyPair]"
                      codePage="1252"
                      dataType="str"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[CurrencyPair]"
                      length="50"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[CurrencyPair]"
                      name="CurrencyPair"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateDateTime]"
                      codePage="1252"
                      dataType="str"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[RateDateTime]"
                      length="50"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateDateTime]"
                      name="RateDateTime"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateBid]"
                      codePage="1252"
                      dataType="str"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[RateBid]"
                      length="50"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateBid]"
                      name="RateBid"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateAsk]"
                      codePage="1252"
                      dataType="str"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[RateAsk]"
                      length="50"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[RateAsk]"
                      name="RateAsk"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[cDealable]"
                      codePage="1252"
                      dataType="str"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[cDealable]"
                      length="50"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[cDealable]"
                      name="cDealable"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]"
                      dataType="cy"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[Spread]"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[Spread]"
                      name="Spread"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[MidRate]"
                      dataType="numeric"
                      errorOrTruncationOperation="Conversion"
                      errorRowDisposition="FailComponent"
                      externalMetadataColumnId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[MidRate]"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].Columns[MidRate]"
                      name="MidRate"
                      precision="30"
                      scale="15"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                          name="FastParse">false</property>
                        <property
                          dataType="System.Boolean"
                          description="Indicates whether the data is in binary format."
                          name="UseBinaryFormat">false</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns
                    isUsed="True">
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[lTid]"
                      codePage="1252"
                      dataType="str"
                      length="50"
                      name="lTid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[CurrencyPair]"
                      codePage="1252"
                      dataType="str"
                      length="50"
                      name="CurrencyPair" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[RateDateTime]"
                      codePage="1252"
                      dataType="str"
                      length="50"
                      name="RateDateTime" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[RateBid]"
                      codePage="1252"
                      dataType="str"
                      length="50"
                      name="RateBid" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[RateAsk]"
                      codePage="1252"
                      dataType="str"
                      length="50"
                      name="RateAsk" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[cDealable]"
                      codePage="1252"
                      dataType="str"
                      length="50"
                      name="cDealable" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[Spread]"
                      dataType="cy"
                      name="Spread" />
                    <externalMetadataColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output].ExternalColumns[MidRate]"
                      dataType="numeric"
                      name="MidRate"
                      precision="30"
                      scale="15" />
                  </externalMetadataColumns>
                </output>
                <output
                  refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Error Output]"
                  isErrorOut="true"
                  name="Flat File Source Error Output">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Error Output].Columns[Flat File Source Error Output Column]"
                      codePage="1252"
                      dataType="text"
                      description="Flat File Source Error Output Column"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Error Output].Columns[Flat File Source Error Output Column]"
                      name="Flat File Source Error Output Column" />
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Error Output].Columns[ErrorCode]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Error Output].Columns[ErrorCode]"
                      name="ErrorCode"
                      specialFlags="1" />
                    <outputColumn
                      refId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Error Output].Columns[ErrorColumn]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Error Output].Columns[ErrorColumn]"
                      name="ErrorColumn"
                      specialFlags="2" />
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Multicast"
              componentClassID="Microsoft.Multicast"
              contactInfo="Multicast;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
              description="Distributes every input row to every row in one or more outputs. For example, branch your data flow to make a copy of data so that some values can be masked before sharing with external partners."
              name="Multicast">
              <inputs>
                <input
                  refId="Package\Data Flow Task\Multicast.Inputs[Multicast Input 1]"
                  name="Multicast Input 1">
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Multicast.Outputs[Multicast Output 1]"
                  deleteOutputOnPathDetached="true"
                  name="Multicast Output 1"
                  synchronousInputId="Package\Data Flow Task\Multicast.Inputs[Multicast Input 1]">
                  <externalMetadataColumns />
                </output>
                <output
                  refId="Package\Data Flow Task\Multicast.Outputs[Multicast Output 2]"
                  deleteOutputOnPathDetached="true"
                  name="Multicast Output 2"
                  synchronousInputId="Package\Data Flow Task\Multicast.Inputs[Multicast Input 1]">
                  <externalMetadataColumns />
                </output>
                <output
                  refId="Package\Data Flow Task\Multicast.Outputs[Multicast Output 3]"
                  deleteOutputOnPathDetached="true"
                  name="Multicast Output 3"
                  synchronousInputId="Package\Data Flow Task\Multicast.Inputs[Multicast Input 1]">
                  <externalMetadataColumns />
                </output>
                <output
                  refId="Package\Data Flow Task\Multicast.Outputs[Multicast Output 4]"
                  dangling="true"
                  deleteOutputOnPathDetached="true"
                  name="Multicast Output 4"
                  synchronousInputId="Package\Data Flow Task\Multicast.Inputs[Multicast Input 1]">
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Sort Daily"
              componentClassID="Microsoft.Sort"
              contactInfo="Sort;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;1"
              description="Sorts input data in ascending or descending order when it cannot be sorted at its source. For example, sort sales data by 'customer id' before it is written to a flat file and delivered to another department. Note: We do not recommend this transformation for large data flows."
              name="Sort Daily"
              version="1">
              <properties>
                <property
                  dataType="System.Boolean"
                  description="Indicates whether the Sort transformation removes rows with duplicate sort values."
                  name="EliminateDuplicates">false</property>
                <property
                  dataType="System.Int32"
                  description="Specifies the maximum number of threads to use for sorting."
                  expressionType="Notify"
                  name="MaximumThreads">-1</property>
              </properties>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input]"
                  name="Sort Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[AvgRateBid]"
                      cachedDataType="cy"
                      cachedName="AvgRateBid"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[AvgRateAsk]"
                      cachedDataType="cy"
                      cachedName="AvgRateAsk"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[AvgMidRate]"
                      cachedDataType="cy"
                      cachedName="AvgMidRate"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[AvgSpread]"
                      cachedDataType="cy"
                      cachedName="AvgSpread"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MinRateBid]"
                      cachedDataType="cy"
                      cachedName="MinRateBid"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MinRateAsk]"
                      cachedDataType="cy"
                      cachedName="MinRateAsk"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MinMidRate]"
                      cachedDataType="cy"
                      cachedName="MinMidRate"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MinSpread]"
                      cachedDataType="cy"
                      cachedName="MinSpread"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MaxRateBid]"
                      cachedDataType="cy"
                      cachedName="MaxRateBid"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MaxRateAsk]"
                      cachedDataType="cy"
                      cachedName="MaxRateAsk"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MaxMidRate]"
                      cachedDataType="cy"
                      cachedName="MaxMidRate"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[MaxSpread]"
                      cachedDataType="cy"
                      cachedName="MaxSpread"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input].Columns[Daily]"
                      cachedDataType="wstr"
                      cachedLength="10"
                      cachedName="Daily"
                      lineageId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[Daily]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">-1</property>
                      </properties>
                    </inputColumn>
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output]"
                  isSorted="true"
                  name="Sort Output">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgRateBid]"
                      name="AvgRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgRateAsk]"
                      name="AvgRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgMidRate]"
                      name="AvgMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[AvgSpread]"
                      name="AvgSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[AvgSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinRateBid]"
                      name="MinRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinRateAsk]"
                      name="MinRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinMidRate]"
                      name="MinMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MinSpread]"
                      name="MinSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MinSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxRateBid]"
                      name="MaxRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxRateAsk]"
                      name="MaxRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxMidRate]"
                      name="MaxMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[MaxSpread]"
                      name="MaxSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[MaxSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[Daily]"
                      dataType="wstr"
                      length="10"
                      lineageId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output].Columns[Daily]"
                      name="Daily"
                      sortKeyPosition="-1">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1].Columns[Daily]}</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Sort Monthly"
              componentClassID="Microsoft.Sort"
              contactInfo="Sort;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;1"
              description="Sorts input data in ascending or descending order when it cannot be sorted at its source. For example, sort sales data by 'customer id' before it is written to a flat file and delivered to another department. Note: We do not recommend this transformation for large data flows."
              name="Sort Monthly"
              version="1">
              <properties>
                <property
                  dataType="System.Boolean"
                  description="Indicates whether the Sort transformation removes rows with duplicate sort values."
                  name="EliminateDuplicates">false</property>
                <property
                  dataType="System.Int32"
                  description="Specifies the maximum number of threads to use for sorting."
                  expressionType="Notify"
                  name="MaximumThreads">-1</property>
              </properties>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input]"
                  name="Sort Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[Monthly]"
                      cachedDataType="wstr"
                      cachedLength="7"
                      cachedName="Monthly"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[Monthly]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">-1</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[AvgRateBid]"
                      cachedDataType="cy"
                      cachedName="AvgRateBid"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[AvgRateAsk]"
                      cachedDataType="cy"
                      cachedName="AvgRateAsk"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[AvgMidRate]"
                      cachedDataType="cy"
                      cachedName="AvgMidRate"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[AvgSpread]"
                      cachedDataType="cy"
                      cachedName="AvgSpread"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MinRateBid]"
                      cachedDataType="cy"
                      cachedName="MinRateBid"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MinRateAsk]"
                      cachedDataType="cy"
                      cachedName="MinRateAsk"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MinMidRate]"
                      cachedDataType="cy"
                      cachedName="MinMidRate"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MinSpread]"
                      cachedDataType="cy"
                      cachedName="MinSpread"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MaxRateBid]"
                      cachedDataType="cy"
                      cachedName="MaxRateBid"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MaxRateAsk]"
                      cachedDataType="cy"
                      cachedName="MaxRateAsk"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MaxMidRate]"
                      cachedDataType="cy"
                      cachedName="MaxMidRate"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input].Columns[MaxSpread]"
                      cachedDataType="cy"
                      cachedName="MaxSpread"
                      lineageId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output]"
                  isSorted="true"
                  name="Sort Output">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[Monthly]"
                      dataType="wstr"
                      length="7"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[Monthly]"
                      name="Monthly"
                      sortKeyPosition="-1">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[Monthly]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgRateBid]"
                      name="AvgRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgRateAsk]"
                      name="AvgRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgMidRate]"
                      name="AvgMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[AvgSpread]"
                      name="AvgSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[AvgSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinRateBid]"
                      name="MinRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinRateAsk]"
                      name="MinRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinMidRate]"
                      name="MinMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MinSpread]"
                      name="MinSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MinSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxRateBid]"
                      name="MaxRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxRateAsk]"
                      name="MaxRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxMidRate]"
                      name="MaxMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output].Columns[MaxSpread]"
                      name="MaxSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1].Columns[MaxSpread]}</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
            <component
              refId="Package\Data Flow Task\Sort Yearly"
              componentClassID="Microsoft.Sort"
              contactInfo="Sort;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;1"
              description="Sorts input data in ascending or descending order when it cannot be sorted at its source. For example, sort sales data by 'customer id' before it is written to a flat file and delivered to another department. Note: We do not recommend this transformation for large data flows."
              name="Sort Yearly"
              version="1">
              <properties>
                <property
                  dataType="System.Boolean"
                  description="Indicates whether the Sort transformation removes rows with duplicate sort values."
                  name="EliminateDuplicates">false</property>
                <property
                  dataType="System.Int32"
                  description="Specifies the maximum number of threads to use for sorting."
                  expressionType="Notify"
                  name="MaximumThreads">-1</property>
              </properties>
              <inputs>
                <input
                  refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input]"
                  name="Sort Input">
                  <inputColumns>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[Yearly]"
                      cachedDataType="i4"
                      cachedName="Yearly"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[Yearly]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">-1</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[AvgRateBid]"
                      cachedDataType="cy"
                      cachedName="AvgRateBid"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[AvgRateAsk]"
                      cachedDataType="cy"
                      cachedName="AvgRateAsk"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[AvgSpread]"
                      cachedDataType="cy"
                      cachedName="AvgSpread"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[AvgMidRate]"
                      cachedDataType="cy"
                      cachedName="AvgMidRate"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MinRateBid]"
                      cachedDataType="cy"
                      cachedName="MinRateBid"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MinRateAsk]"
                      cachedDataType="cy"
                      cachedName="MinRateAsk"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MinSpread]"
                      cachedDataType="cy"
                      cachedName="MinSpread"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MinMidRate]"
                      cachedDataType="cy"
                      cachedName="MinMidRate"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MaxRateBid]"
                      cachedDataType="cy"
                      cachedName="MaxRateBid"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateBid]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MaxRateAsk]"
                      cachedDataType="cy"
                      cachedName="MaxRateAsk"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MaxSpread]"
                      cachedDataType="cy"
                      cachedName="MaxSpread"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxSpread]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                    <inputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input].Columns[MaxMidRate]"
                      cachedDataType="cy"
                      cachedName="MaxMidRate"
                      lineageId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxMidRate]">
                      <properties>
                        <property
                          dataType="System.Int32"
                          description="Specifies the comparison options for character data."
                          name="NewComparisonFlags">0</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the sort order of the column."
                          name="NewSortKeyPosition">0</property>
                      </properties>
                    </inputColumn>
                  </inputColumns>
                  <externalMetadataColumns />
                </input>
              </inputs>
              <outputs>
                <output
                  refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output]"
                  isSorted="true"
                  name="Sort Output">
                  <outputColumns>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[Yearly]"
                      dataType="i4"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[Yearly]"
                      name="Yearly"
                      sortKeyPosition="-1">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[Yearly]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgRateBid]"
                      name="AvgRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgRateAsk]"
                      name="AvgRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgSpread]"
                      name="AvgSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[AvgMidRate]"
                      name="AvgMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[AvgMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinRateBid]"
                      name="MinRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinRateAsk]"
                      name="MinRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinSpread]"
                      name="MinSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MinMidRate]"
                      name="MinMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MinMidRate]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxRateBid]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxRateBid]"
                      name="MaxRateBid">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateBid]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxRateAsk]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxRateAsk]"
                      name="MaxRateAsk">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxRateAsk]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxSpread]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxSpread]"
                      name="MaxSpread">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxSpread]}</property>
                      </properties>
                    </outputColumn>
                    <outputColumn
                      refId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxMidRate]"
                      dataType="cy"
                      lineageId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output].Columns[MaxMidRate]"
                      name="MaxMidRate">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.Int32"
                          description="Specifies the lineage identifier of the input column that is associated with this output column."
                          name="SortColumnId">#{Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1].Columns[MaxMidRate]}</property>
                      </properties>
                    </outputColumn>
                  </outputColumns>
                  <externalMetadataColumns />
                </output>
              </outputs>
            </component>
          </components>
          <paths>
            <path
              refId="Package\Data Flow Task.Paths[Aggregate Output 1]"
              endId="Package\Data Flow Task\Sort Monthly.Inputs[Sort Input]"
              name="Aggregate Output 1"
              startId="Package\Data Flow Task\Data Monthly.Outputs[Aggregate Output 1]" />
            <path
              refId="Package\Data Flow Task.Paths[Aggregate Output 11]"
              endId="Package\Data Flow Task\Sort Yearly.Inputs[Sort Input]"
              name="Aggregate Output 1"
              startId="Package\Data Flow Task\Data Yearly.Outputs[Aggregate Output 1]" />
            <path
              refId="Package\Data Flow Task.Paths[Aggregate Output 12]"
              endId="Package\Data Flow Task\Sort Daily.Inputs[Sort Input]"
              name="Aggregate Output 1"
              startId="Package\Data Flow Task\Data Daily.Outputs[Aggregate Output 1]" />
            <path
              refId="Package\Data Flow Task.Paths[Data Conversion Output]"
              endId="Package\Data Flow Task\Derived Column.Inputs[Derived Column Input]"
              name="Data Conversion Output"
              startId="Package\Data Flow Task\Data Conversion.Outputs[Data Conversion Output]" />
            <path
              refId="Package\Data Flow Task.Paths[Derived Column Output]"
              endId="Package\Data Flow Task\Multicast.Inputs[Multicast Input 1]"
              name="Derived Column Output"
              startId="Package\Data Flow Task\Derived Column.Outputs[Derived Column Output]" />
            <path
              refId="Package\Data Flow Task.Paths[Flat File Source Output]"
              endId="Package\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]"
              name="Flat File Source Output"
              startId="Package\Data Flow Task\Flat File Source.Outputs[Flat File Source Output]" />
            <path
              refId="Package\Data Flow Task.Paths[Multicast Output 1]"
              endId="Package\Data Flow Task\Data Yearly.Inputs[Aggregate Input 1]"
              name="Multicast Output 1"
              startId="Package\Data Flow Task\Multicast.Outputs[Multicast Output 1]" />
            <path
              refId="Package\Data Flow Task.Paths[Multicast Output 2]"
              endId="Package\Data Flow Task\Data Monthly.Inputs[Aggregate Input 1]"
              name="Multicast Output 2"
              startId="Package\Data Flow Task\Multicast.Outputs[Multicast Output 2]" />
            <path
              refId="Package\Data Flow Task.Paths[Multicast Output 3]"
              endId="Package\Data Flow Task\Data Daily.Inputs[Aggregate Input 1]"
              name="Multicast Output 3"
              startId="Package\Data Flow Task\Multicast.Outputs[Multicast Output 3]" />
            <path
              refId="Package\Data Flow Task.Paths[Sort Output]"
              endId="Package\Data Flow Task\Data Destination Monthly.Inputs[Flat File Destination Input]"
              name="Sort Output"
              startId="Package\Data Flow Task\Sort Monthly.Outputs[Sort Output]" />
            <path
              refId="Package\Data Flow Task.Paths[Sort Output1]"
              endId="Package\Data Flow Task\Data Destination Yearly.Inputs[Flat File Destination Input]"
              name="Sort Output"
              startId="Package\Data Flow Task\Sort Yearly.Outputs[Sort Output]" />
            <path
              refId="Package\Data Flow Task.Paths[Sort Output2]"
              endId="Package\Data Flow Task\Data Destination Daily.Inputs[Flat File Destination Input]"
              name="Sort Output"
              startId="Package\Data Flow Task\Sort Daily.Outputs[Sort Output]" />
          </paths>
        </pipeline>
      </DTS:ObjectData>
    </DTS:Executable>
    <DTS:Executable
      DTS:refId="Package\Foreach Loop Container"
      DTS:CreationName="STOCK:FOREACHLOOP"
      DTS:Description="Foreach Loop Container"
      DTS:DTSID="{89321591-08EA-4AC2-BB38-81767D9525BF}"
      DTS:ExecutableType="STOCK:FOREACHLOOP"
      DTS:LocaleID="-1"
      DTS:ObjectName="Foreach Loop Container">
      <DTS:ForEachEnumerator
        DTS:CreationName="Microsoft.ForEachFileEnumerator"
        DTS:DTSID="{EEAD0825-BF7A-42EE-8FAC-AF68494DD7C3}"
        DTS:ObjectName="{EEAD0825-BF7A-42EE-8FAC-AF68494DD7C3}">
        <DTS:ObjectData>
          <ForEachFileEnumeratorProperties>
            <FEFEProperty
              Folder="E:\BigData\DataSource" />
            <FEFEProperty
              FileSpec="*.csv" />
            <FEFEProperty
              FileNameRetrievalType="0" />
            <FEFEProperty
              Recurse="0" />
          </ForEachFileEnumeratorProperties>
        </DTS:ObjectData>
      </DTS:ForEachEnumerator>
      <DTS:Variables />
      <DTS:Executables>
        <DTS:Executable
          DTS:refId="Package\Foreach Loop Container\Data Flow Task"
          DTS:CreationName="Microsoft.Pipeline"
          DTS:Description="Data Flow Task"
          DTS:DTSID="{C1B75900-8E83-4018-93D2-FDA60A832209}"
          DTS:ExecutableType="Microsoft.Pipeline"
          DTS:LocaleID="-1"
          DTS:ObjectName="Data Flow Task"
          DTS:TaskContact="Performs high-performance data extraction, transformation and loading;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved;http://www.microsoft.com/sql/support/default.asp;1">
          <DTS:Variables />
          <DTS:ObjectData>
            <pipeline
              version="1">
              <components>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion"
                  componentClassID="Microsoft.DataConvert"
                  contactInfo="Data Conversion;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Data Conversion"
                  name="Data Conversion"
                  usesDispositions="true">
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]"
                      name="Data Conversion Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]" />
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output]"
                      exclusionGroup="1"
                      name="Data Conversion Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of lTid]"
                          dataType="numeric"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="RedirectRow"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of lTid]"
                          name="Copy of lTid"
                          precision="18"
                          truncationRowDisposition="RedirectRow">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the input column used as the source of data for the conversion."
                              name="SourceInputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]}</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]"
                          dataType="dbTimeStamp"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="RedirectRow"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]"
                          name="Copy of RateDateTime"
                          truncationRowDisposition="RedirectRow">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the input column used as the source of data for the conversion."
                              name="SourceInputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]}</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]"
                          dataType="cy"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="RedirectRow"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]"
                          name="Copy of RateBid"
                          truncationRowDisposition="RedirectRow">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the input column used as the source of data for the conversion."
                              name="SourceInputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]}</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]"
                          dataType="cy"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="RedirectRow"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]"
                          name="Copy of RateAsk"
                          truncationRowDisposition="RedirectRow">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the input column used as the source of data for the conversion."
                              name="SourceInputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]}</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                          </properties>
                        </outputColumn>
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output]"
                      exclusionGroup="1"
                      isErrorOut="true"
                      name="Data Conversion Error Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorCode]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorCode]"
                          name="ErrorCode"
                          specialFlags="1" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorColumn]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output].Columns[ErrorColumn]"
                          name="ErrorColumn"
                          specialFlags="2" />
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data Destination"
                  componentClassID="Microsoft.FlatFileDestination"
                  contactInfo="Flat File Destination;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Flat File Destination"
                  localeId="1033"
                  name="Data Destination">
                  <properties>
                    <property
                      dataType="System.Boolean"
                      description="Specifies whether the data will overwrite or append to the destination file."
                      name="Overwrite">true</property>
                    <property
                      dataType="System.Null"
                      description="Specifies the text to write to the destination file before any data is written."
                      expressionType="Notify"
                      name="Header" />
                  </properties>
                  <connections>
                    <connection
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Connections[FlatFileConnection]"
                      connectionManagerID="Package.ConnectionManagers[DataDestinationConnection]"
                      connectionManagerRefId="Package.ConnectionManagers[DataDestinationConnection]"
                      name="FlatFileConnection" />
                  </connections>
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input]"
                      hasSideEffects="true"
                      name="Flat File Destination Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[Copy of RateDateTime]"
                          cachedDataType="dbTimeStamp"
                          cachedName="Copy of RateDateTime"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[Copy of lTid]"
                          cachedDataType="numeric"
                          cachedName="Copy of lTid"
                          cachedPrecision="18"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[Copy of RateBid]"
                          cachedDataType="cy"
                          cachedName="Copy of RateBid"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[Copy of RateAsk]"
                          cachedDataType="cy"
                          cachedName="Copy of RateAsk"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[Spread]"
                          cachedDataType="cy"
                          cachedName="Spread"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[Spread]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Spread]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].Columns[MidRate]"
                          cachedDataType="numeric"
                          cachedName="MidRate"
                          cachedPrecision="30"
                          cachedScale="15"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[MidRate]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[MidRate]" />
                      </inputColumns>
                      <externalMetadataColumns
                        isUsed="True">
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="lTid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="CurrencyPair" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateDateTime" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateBid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateAsk" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="cDealable" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[Spread]"
                          dataType="cy"
                          name="Spread" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input].ExternalColumns[MidRate]"
                          dataType="numeric"
                          name="MidRate"
                          precision="30"
                          scale="15" />
                      </externalMetadataColumns>
                    </input>
                  </inputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING"
                  componentClassID="Microsoft.ConditionalSplit"
                  contactInfo="Conditional Split;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Routes data rows to different outputs depending on the content of the data. Use conditions (SSIS expressions) to specify which rows are routed. For example, separate records that need to be cleaned from those that are ready to be loaded or route only a subset of records."
                  name="Data EMPTY STRING"
                  usesDispositions="true">
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input]"
                      description="Input to the Conditional Split Transformation"
                      name="Conditional Split Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]" />
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[EMPTY_STRING]"
                      description="Output 1 of the Conditional Split Transformation"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      exclusionGroup="1"
                      name="EMPTY_STRING"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input]"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the expression. This expression version uses lineage identifiers instead of column names."
                          name="Expression">[TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]}) == "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]}) == "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]}) == "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]}) == "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]}) == "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]}) == ""</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the friendly version of the expression. This expression version uses column names."
                          expressionType="Notify"
                          name="FriendlyExpression">TRIM(lTid) == "" || TRIM(CurrencyPair) == "" || TRIM(RateDateTime) == "" || TRIM(RateBid) == "" || TRIM(RateAsk) == "" || TRIM(cDealable) == ""</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the position of the condition in the list of conditions that the transformation evaluates. The evaluation order is from the lowest to the highest value."
                          name="EvaluationOrder">0</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[NOT_EMPTY_STRING]"
                      description="Output 2 of the Conditional Split Transformation"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      exclusionGroup="1"
                      name="NOT_EMPTY_STRING"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input]"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the expression. This expression version uses lineage identifiers instead of column names."
                          name="Expression">[TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]}) != "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]}) != "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]}) != "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]}) != "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]}) != "" || [TRIM](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]}) != ""</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the friendly version of the expression. This expression version uses column names."
                          expressionType="Notify"
                          name="FriendlyExpression">TRIM(lTid) != "" || TRIM(CurrencyPair) != "" || TRIM(RateDateTime) != "" || TRIM(RateBid) != "" || TRIM(RateAsk) != "" || TRIM(cDealable) != ""</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the position of the condition in the list of conditions that the transformation evaluates. The evaluation order is from the lowest to the highest value."
                          name="EvaluationOrder">1</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[Conditional Split Default Output]"
                      description="Default Output of the Conditional Split Transformation"
                      exclusionGroup="1"
                      name="Conditional Split Default Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input]">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          name="IsDefaultOut">true</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[Conditional Split Error Output]"
                      description="Error Output of the Conditional Split Transformation"
                      exclusionGroup="1"
                      isErrorOut="true"
                      name="Conditional Split Error Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input]">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[Conditional Split Error Output].Columns[ErrorCode]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[Conditional Split Error Output].Columns[ErrorCode]"
                          name="ErrorCode"
                          specialFlags="1" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[Conditional Split Error Output].Columns[ErrorColumn]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[Conditional Split Error Output].Columns[ErrorColumn]"
                          name="ErrorColumn"
                          specialFlags="2" />
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data Error"
                  componentClassID="Microsoft.FlatFileDestination"
                  contactInfo="Flat File Destination;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Flat File Destination"
                  localeId="1033"
                  name="Data Error">
                  <properties>
                    <property
                      dataType="System.Boolean"
                      description="Specifies whether the data will overwrite or append to the destination file."
                      name="Overwrite">true</property>
                    <property
                      dataType="System.Null"
                      description="Specifies the text to write to the destination file before any data is written."
                      expressionType="Notify"
                      name="Header" />
                  </properties>
                  <connections>
                    <connection
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Connections[FlatFileConnection]"
                      connectionManagerID="Package.ConnectionManagers[DataErrorConnection]"
                      connectionManagerRefId="Package.ConnectionManagers[DataErrorConnection]"
                      name="FlatFileConnection" />
                  </connections>
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input]"
                      hasSideEffects="true"
                      name="Flat File Destination Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]" />
                      </inputColumns>
                      <externalMetadataColumns
                        isUsed="True">
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="lTid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="CurrencyPair" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateDateTime" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateBid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateAsk" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="cDealable" />
                      </externalMetadataColumns>
                    </input>
                  </inputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data NULL"
                  componentClassID="Microsoft.FlatFileDestination"
                  contactInfo="Flat File Destination;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Flat File Destination"
                  localeId="1033"
                  name="Data NULL">
                  <properties>
                    <property
                      dataType="System.Boolean"
                      description="Specifies whether the data will overwrite or append to the destination file."
                      name="Overwrite">true</property>
                    <property
                      dataType="System.Null"
                      description="Specifies the text to write to the destination file before any data is written."
                      expressionType="Notify"
                      name="Header" />
                  </properties>
                  <connections>
                    <connection
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Connections[FlatFileConnection]"
                      connectionManagerID="Package.ConnectionManagers[DataNullConnection]"
                      connectionManagerRefId="Package.ConnectionManagers[DataNullConnection]"
                      name="FlatFileConnection" />
                  </connections>
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input]"
                      hasSideEffects="true"
                      name="Flat File Destination Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[CurrencyPair]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateAsk]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[cDealable]" />
                      </inputColumns>
                      <externalMetadataColumns
                        isUsed="True">
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="lTid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="CurrencyPair" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateDateTime" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateBid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateAsk" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="cDealable" />
                      </externalMetadataColumns>
                    </input>
                  </inputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING"
                  componentClassID="Microsoft.ConditionalSplit"
                  contactInfo="Conditional Split;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Routes data rows to different outputs depending on the content of the data. Use conditions (SSIS expressions) to specify which rows are routed. For example, separate records that need to be cleaned from those that are ready to be loaded or route only a subset of records."
                  name="Data NULL STRING"
                  usesDispositions="true">
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input]"
                      description="Input to the Conditional Split Transformation"
                      name="Conditional Split Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]" />
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[NULL_STRING]"
                      description="Output 1 of the Conditional Split Transformation"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      exclusionGroup="1"
                      name="NULL_STRING"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input]"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the expression. This expression version uses lineage identifiers instead of column names."
                          name="Expression">[LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]}) == "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]}) == "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]}) == "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]}) == "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]}) == "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]}) == "null"</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the friendly version of the expression. This expression version uses column names."
                          expressionType="Notify"
                          name="FriendlyExpression">LOWER(lTid) == "null" || LOWER(CurrencyPair) == "null" || LOWER(RateDateTime) == "null" || LOWER(RateBid) == "null" || LOWER(RateAsk) == "null" || LOWER(cDealable) == "null"</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the position of the condition in the list of conditions that the transformation evaluates. The evaluation order is from the lowest to the highest value."
                          name="EvaluationOrder">0</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[NOT_NULL_STRING]"
                      description="Output 2 of the Conditional Split Transformation"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      exclusionGroup="1"
                      name="NOT_NULL_STRING"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input]"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the expression. This expression version uses lineage identifiers instead of column names."
                          name="Expression">[LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]}) != "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]}) != "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]}) != "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]}) != "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]}) != "null" || [LOWER](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]}) != "null"</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the friendly version of the expression. This expression version uses column names."
                          expressionType="Notify"
                          name="FriendlyExpression">LOWER(lTid) != "null" || LOWER(CurrencyPair) != "null" || LOWER(RateDateTime) != "null" || LOWER(RateBid) != "null" || LOWER(RateAsk) != "null" || LOWER(cDealable) != "null"</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the position of the condition in the list of conditions that the transformation evaluates. The evaluation order is from the lowest to the highest value."
                          name="EvaluationOrder">1</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[Conditional Split Default Output]"
                      description="Default Output of the Conditional Split Transformation"
                      exclusionGroup="1"
                      name="Conditional Split Default Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input]">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          name="IsDefaultOut">true</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[Conditional Split Error Output]"
                      description="Error Output of the Conditional Split Transformation"
                      exclusionGroup="1"
                      isErrorOut="true"
                      name="Conditional Split Error Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input]">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[Conditional Split Error Output].Columns[ErrorCode]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[Conditional Split Error Output].Columns[ErrorCode]"
                          name="ErrorCode"
                          specialFlags="1" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[Conditional Split Error Output].Columns[ErrorColumn]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[Conditional Split Error Output].Columns[ErrorColumn]"
                          name="ErrorColumn"
                          specialFlags="2" />
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE"
                  componentClassID="Microsoft.ConditionalSplit"
                  contactInfo="Conditional Split;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Routes data rows to different outputs depending on the content of the data. Use conditions (SSIS expressions) to specify which rows are routed. For example, separate records that need to be cleaned from those that are ready to be loaded or route only a subset of records."
                  name="Data NULL VALUE"
                  usesDispositions="true">
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input]"
                      description="Input to the Conditional Split Transformation"
                      name="Conditional Split Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]" />
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[NULL_VALUE]"
                      description="Output 1 of the Conditional Split Transformation"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      exclusionGroup="1"
                      name="NULL_VALUE"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input]"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the expression. This expression version uses lineage identifiers instead of column names."
                          name="Expression">[ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]}) || [ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]}) || [ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]}) || [ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]}) || [ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]}) || [ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]})</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the friendly version of the expression. This expression version uses column names."
                          expressionType="Notify"
                          name="FriendlyExpression">ISNULL(lTid) || ISNULL(CurrencyPair) || ISNULL(RateDateTime) || ISNULL(RateBid) || ISNULL(RateAsk) || ISNULL(cDealable)</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the position of the condition in the list of conditions that the transformation evaluates. The evaluation order is from the lowest to the highest value."
                          name="EvaluationOrder">0</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[NOTNULL_VALUE]"
                      description="Output 2 of the Conditional Split Transformation"
                      errorOrTruncationOperation="Computation"
                      errorRowDisposition="FailComponent"
                      exclusionGroup="1"
                      name="NOTNULL_VALUE"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input]"
                      truncationRowDisposition="FailComponent">
                      <properties>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the expression. This expression version uses lineage identifiers instead of column names."
                          name="Expression">![ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]}) &amp;&amp; ![ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]}) &amp;&amp; ![ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]}) &amp;&amp; ![ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]}) &amp;&amp; ![ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]}) &amp;&amp; ![ISNULL](#{Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]})</property>
                        <property
                          containsID="true"
                          dataType="System.String"
                          description="Specifies the friendly version of the expression. This expression version uses column names."
                          expressionType="Notify"
                          name="FriendlyExpression">!ISNULL(lTid) &amp;&amp; !ISNULL(CurrencyPair) &amp;&amp; !ISNULL(RateDateTime) &amp;&amp; !ISNULL(RateBid) &amp;&amp; !ISNULL(RateAsk) &amp;&amp; !ISNULL(cDealable)</property>
                        <property
                          dataType="System.Int32"
                          description="Specifies the position of the condition in the list of conditions that the transformation evaluates. The evaluation order is from the lowest to the highest value."
                          name="EvaluationOrder">1</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[Conditional Split Default Output]"
                      description="Default Output of the Conditional Split Transformation"
                      exclusionGroup="1"
                      name="Conditional Split Default Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input]">
                      <properties>
                        <property
                          dataType="System.Boolean"
                          name="IsDefaultOut">true</property>
                      </properties>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[Conditional Split Error Output]"
                      description="Error Output of the Conditional Split Transformation"
                      exclusionGroup="1"
                      isErrorOut="true"
                      name="Conditional Split Error Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input]">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[Conditional Split Error Output].Columns[ErrorCode]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[Conditional Split Error Output].Columns[ErrorCode]"
                          name="ErrorCode"
                          specialFlags="1" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[Conditional Split Error Output].Columns[ErrorColumn]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[Conditional Split Error Output].Columns[ErrorColumn]"
                          name="ErrorColumn"
                          specialFlags="2" />
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Data Source"
                  componentClassID="Microsoft.FlatFileSource"
                  contactInfo="Flat File Source;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;1"
                  description="Flat File Source"
                  localeId="1033"
                  name="Data Source"
                  usesDispositions="true"
                  version="1">
                  <properties>
                    <property
                      dataType="System.Boolean"
                      description="Specifies whether zero-length columns are treated as null."
                      name="RetainNulls">true</property>
                    <property
                      dataType="System.String"
                      description="Specifies the name of an output column containing the file name. If no name is specified, no output column containing the file name will be generated."
                      name="FileNameColumnName"></property>
                  </properties>
                  <connections>
                    <connection
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Connections[FlatFileConnection]"
                      connectionManagerID="Package.ConnectionManagers[DataSourceConnection]"
                      connectionManagerRefId="Package.ConnectionManagers[DataSourceConnection]"
                      name="FlatFileConnection" />
                  </connections>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output]"
                      name="Flat File Source Output">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[lTid]"
                          codePage="1252"
                          dataType="str"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="FailComponent"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 0]"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[lTid]"
                          name="lTid"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the data is in binary format."
                              name="UseBinaryFormat">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[CurrencyPair]"
                          codePage="1252"
                          dataType="str"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="FailComponent"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 1]"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[CurrencyPair]"
                          name="CurrencyPair"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the data is in binary format."
                              name="UseBinaryFormat">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateDateTime]"
                          codePage="1252"
                          dataType="str"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="FailComponent"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 2]"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateDateTime]"
                          name="RateDateTime"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the data is in binary format."
                              name="UseBinaryFormat">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateBid]"
                          codePage="1252"
                          dataType="str"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="FailComponent"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 3]"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateBid]"
                          name="RateBid"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the data is in binary format."
                              name="UseBinaryFormat">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateAsk]"
                          codePage="1252"
                          dataType="str"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="FailComponent"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 4]"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateAsk]"
                          name="RateAsk"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the data is in binary format."
                              name="UseBinaryFormat">false</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[cDealable]"
                          codePage="1252"
                          dataType="str"
                          errorOrTruncationOperation="Conversion"
                          errorRowDisposition="FailComponent"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 5]"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[cDealable]"
                          name="cDealable"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the column uses the faster, locale-neutral parsing routines."
                              name="FastParse">false</property>
                            <property
                              dataType="System.Boolean"
                              description="Indicates whether the data is in binary format."
                              name="UseBinaryFormat">false</property>
                          </properties>
                        </outputColumn>
                      </outputColumns>
                      <externalMetadataColumns
                        isUsed="True">
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 0]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="Column 0" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 1]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="Column 1" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 2]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="Column 2" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 3]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="Column 3" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 4]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="Column 4" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].ExternalColumns[Column 5]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="Column 5" />
                      </externalMetadataColumns>
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Error Output]"
                      isErrorOut="true"
                      name="Flat File Source Error Output">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Error Output].Columns[Flat File Source Error Output Column]"
                          codePage="1252"
                          dataType="text"
                          description="Flat File Source Error Output Column"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Error Output].Columns[Flat File Source Error Output Column]"
                          name="Flat File Source Error Output Column" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Error Output].Columns[ErrorCode]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Error Output].Columns[ErrorCode]"
                          name="ErrorCode"
                          specialFlags="1" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Error Output].Columns[ErrorColumn]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Error Output].Columns[ErrorColumn]"
                          name="ErrorColumn"
                          specialFlags="2" />
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Derived Column"
                  componentClassID="Microsoft.DerivedColumn"
                  contactInfo="Derived Column;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Creates new column values by applying expressions to transformation input columns. Create new columns or overwrite existing ones. For example, concatenate the values from the 'first name' and 'last name' column to make a 'full name' column."
                  name="Derived Column"
                  usesDispositions="true">
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Inputs[Derived Column Input]"
                      description="Input to the Derived Column Transformation"
                      name="Derived Column Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Inputs[Derived Column Input].Columns[Copy of RateBid]"
                          cachedDataType="cy"
                          cachedName="Copy of RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Inputs[Derived Column Input].Columns[Copy of RateAsk]"
                          cachedDataType="cy"
                          cachedName="Copy of RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]" />
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output]"
                      description="Default Output of the Derived Column Transformation"
                      exclusionGroup="1"
                      name="Derived Column Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Inputs[Derived Column Input]">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Spread]"
                          dataType="cy"
                          errorOrTruncationOperation="Computation"
                          errorRowDisposition="FailComponent"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Spread]"
                          name="Spread"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.String"
                              description="Derived Column Expression"
                              name="Expression">[ABS](#{Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]} - #{Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]})</property>
                            <property
                              containsID="true"
                              dataType="System.String"
                              description="Derived Column Friendly Expression"
                              expressionType="Notify"
                              name="FriendlyExpression">ABS([Copy of RateAsk] - [Copy of RateBid])</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[MidRate]"
                          dataType="numeric"
                          errorOrTruncationOperation="Computation"
                          errorRowDisposition="FailComponent"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[MidRate]"
                          name="MidRate"
                          precision="30"
                          scale="15"
                          truncationRowDisposition="FailComponent">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.String"
                              description="Derived Column Expression"
                              name="Expression">(#{Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]} + #{Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]}) / 2</property>
                            <property
                              containsID="true"
                              dataType="System.String"
                              description="Derived Column Friendly Expression"
                              expressionType="Notify"
                              name="FriendlyExpression">([Copy of RateAsk] + [Copy of RateBid]) / 2</property>
                          </properties>
                        </outputColumn>
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Error Output]"
                      description="Error Output of the Derived Column Transformation"
                      exclusionGroup="1"
                      isErrorOut="true"
                      name="Derived Column Error Output"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Inputs[Derived Column Input]">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorCode]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorCode]"
                          name="ErrorCode"
                          specialFlags="1" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorColumn]"
                          dataType="i4"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Error Output].Columns[ErrorColumn]"
                          name="ErrorColumn"
                          specialFlags="2" />
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Multicast"
                  componentClassID="Microsoft.Multicast"
                  contactInfo="Multicast;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Distributes every input row to every row in one or more outputs. For example, branch your data flow to make a copy of data so that some values can be masked before sharing with external partners."
                  name="Multicast">
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Multicast.Inputs[Multicast Input 1]"
                      name="Multicast Input 1">
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Multicast.Outputs[Total]"
                      deleteOutputOnPathDetached="true"
                      name="Total"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Multicast.Inputs[Multicast Input 1]">
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Multicast.Outputs[Multicast Output 2]"
                      deleteOutputOnPathDetached="true"
                      name="Multicast Output 2"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Multicast.Inputs[Multicast Input 1]">
                      <externalMetadataColumns />
                    </output>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Multicast.Outputs[Multicast Output 1]"
                      dangling="true"
                      deleteOutputOnPathDetached="true"
                      name="Multicast Output 1"
                      synchronousInputId="Package\Foreach Loop Container\Data Flow Task\Multicast.Inputs[Multicast Input 1]">
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Sort"
                  componentClassID="Microsoft.Sort"
                  contactInfo="Sort;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;1"
                  description="Sorts input data in ascending or descending order when it cannot be sorted at its source. For example, sort sales data by 'customer id' before it is written to a flat file and delivered to another department. Note: We do not recommend this transformation for large data flows."
                  name="Sort"
                  version="1">
                  <properties>
                    <property
                      dataType="System.Boolean"
                      description="Indicates whether the Sort transformation removes rows with duplicate sort values."
                      name="EliminateDuplicates">false</property>
                    <property
                      dataType="System.Int32"
                      description="Specifies the maximum number of threads to use for sorting."
                      expressionType="Notify"
                      name="MaximumThreads">-1</property>
                  </properties>
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input]"
                      name="Sort Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[lTid]">
                          <properties>
                            <property
                              dataType="System.Int32"
                              description="Specifies the comparison options for character data."
                              name="NewComparisonFlags">0</property>
                            <property
                              dataType="System.Int32"
                              description="Specifies the sort order of the column."
                              name="NewSortKeyPosition">0</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[CurrencyPair]">
                          <properties>
                            <property
                              dataType="System.Int32"
                              description="Specifies the comparison options for character data."
                              name="NewComparisonFlags">0</property>
                            <property
                              dataType="System.Int32"
                              description="Specifies the sort order of the column."
                              name="NewSortKeyPosition">0</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateDateTime]">
                          <properties>
                            <property
                              dataType="System.Int32"
                              description="Specifies the comparison options for character data."
                              name="NewComparisonFlags">0</property>
                            <property
                              dataType="System.Int32"
                              description="Specifies the sort order of the column."
                              name="NewSortKeyPosition">-1</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateBid]">
                          <properties>
                            <property
                              dataType="System.Int32"
                              description="Specifies the comparison options for character data."
                              name="NewComparisonFlags">0</property>
                            <property
                              dataType="System.Int32"
                              description="Specifies the sort order of the column."
                              name="NewSortKeyPosition">0</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateAsk]">
                          <properties>
                            <property
                              dataType="System.Int32"
                              description="Specifies the comparison options for character data."
                              name="NewComparisonFlags">0</property>
                            <property
                              dataType="System.Int32"
                              description="Specifies the sort order of the column."
                              name="NewSortKeyPosition">0</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[cDealable]">
                          <properties>
                            <property
                              dataType="System.Int32"
                              description="Specifies the comparison options for character data."
                              name="NewComparisonFlags">0</property>
                            <property
                              dataType="System.Int32"
                              description="Specifies the sort order of the column."
                              name="NewSortKeyPosition">0</property>
                          </properties>
                        </inputColumn>
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output]"
                      isSorted="true"
                      name="Sort Output">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]"
                          name="lTid">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the lineage identifier of the input column that is associated with this output column."
                              name="SortColumnId">#{Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[lTid]}</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]"
                          name="CurrencyPair">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the lineage identifier of the input column that is associated with this output column."
                              name="SortColumnId">#{Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[CurrencyPair]}</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]"
                          name="RateDateTime"
                          sortKeyPosition="-1">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the lineage identifier of the input column that is associated with this output column."
                              name="SortColumnId">#{Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateDateTime]}</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]"
                          name="RateBid">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the lineage identifier of the input column that is associated with this output column."
                              name="SortColumnId">#{Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateBid]}</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]"
                          name="RateAsk">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the lineage identifier of the input column that is associated with this output column."
                              name="SortColumnId">#{Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[RateAsk]}</property>
                          </properties>
                        </outputColumn>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]"
                          name="cDealable">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Specifies the lineage identifier of the input column that is associated with this output column."
                              name="SortColumnId">#{Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output].Columns[cDealable]}</property>
                          </properties>
                        </outputColumn>
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination"
                  componentClassID="Microsoft.FlatFileDestination"
                  contactInfo="Flat File Destination;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;0"
                  description="Flat File Destination"
                  localeId="1033"
                  name="Total Data Destination">
                  <properties>
                    <property
                      dataType="System.Boolean"
                      description="Specifies whether the data will overwrite or append to the destination file."
                      name="Overwrite">false</property>
                    <property
                      dataType="System.Null"
                      description="Specifies the text to write to the destination file before any data is written."
                      expressionType="Notify"
                      name="Header" />
                  </properties>
                  <connections>
                    <connection
                      refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Connections[FlatFileConnection]"
                      connectionManagerID="Package.ConnectionManagers[DataTotalDestinationConnection]"
                      connectionManagerRefId="Package.ConnectionManagers[DataTotalDestinationConnection]"
                      name="FlatFileConnection" />
                  </connections>
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input]"
                      hasSideEffects="true"
                      name="Flat File Destination Input">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[Copy of lTid]"
                          cachedDataType="numeric"
                          cachedName="Copy of lTid"
                          cachedPrecision="18"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of lTid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[Copy of RateDateTime]"
                          cachedDataType="dbTimeStamp"
                          cachedName="Copy of RateDateTime"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateDateTime]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[Copy of RateBid]"
                          cachedDataType="cy"
                          cachedName="Copy of RateBid"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateBid]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[Copy of RateAsk]"
                          cachedDataType="cy"
                          cachedName="Copy of RateAsk"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output].Columns[Copy of RateAsk]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[Spread]"
                          cachedDataType="cy"
                          cachedName="Spread"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[Spread]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[Spread]" />
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].Columns[MidRate]"
                          cachedDataType="numeric"
                          cachedName="MidRate"
                          cachedPrecision="30"
                          cachedScale="15"
                          externalMetadataColumnId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[MidRate]"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output].Columns[MidRate]" />
                      </inputColumns>
                      <externalMetadataColumns
                        isUsed="True">
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[lTid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="lTid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[CurrencyPair]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="CurrencyPair" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateDateTime]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateDateTime" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateBid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateBid" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[RateAsk]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="RateAsk" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[cDealable]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          name="cDealable" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[Spread]"
                          dataType="cy"
                          name="Spread" />
                        <externalMetadataColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input].ExternalColumns[MidRate]"
                          dataType="numeric"
                          name="MidRate"
                          precision="30"
                          scale="15" />
                      </externalMetadataColumns>
                    </input>
                  </inputs>
                </component>
                <component
                  refId="Package\Foreach Loop Container\Data Flow Task\Union All"
                  componentClassID="Microsoft.UnionAll"
                  contactInfo="Union All;Microsoft Corporation; Microsoft SQL Server; (C) Microsoft Corporation; All Rights Reserved; http://www.microsoft.com/sql/support;1"
                  description="Combines rows from multiple data flows without sorting. For example, add rows back to a data flow after correction of errors. If sorting is important, we recommend using the Merge transformation."
                  name="Union All"
                  version="1">
                  <inputs>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1]"
                      name="Union All Input 1">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[lTid]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[CurrencyPair]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateDateTime]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateBid]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateAsk]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[cDealable]}</property>
                          </properties>
                        </inputColumn>
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2]"
                      hasSideEffects="true"
                      name="Union All Input 2">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[lTid]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[CurrencyPair]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateDateTime]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateBid]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateAsk]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[cDealable]}</property>
                          </properties>
                        </inputColumn>
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3]"
                      hasSideEffects="true"
                      name="Union All Input 3">
                      <inputColumns>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3].Columns[lTid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="lTid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[lTid]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[lTid]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3].Columns[CurrencyPair]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="CurrencyPair"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[CurrencyPair]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[CurrencyPair]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3].Columns[RateDateTime]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateDateTime"
                          cachedSortKeyPosition="-1"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateDateTime]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateDateTime]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3].Columns[RateBid]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateBid"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateBid]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateBid]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3].Columns[RateAsk]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="RateAsk"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[RateAsk]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateAsk]}</property>
                          </properties>
                        </inputColumn>
                        <inputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3].Columns[cDealable]"
                          cachedCodepage="1252"
                          cachedDataType="str"
                          cachedLength="50"
                          cachedName="cDealable"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output].Columns[cDealable]">
                          <properties>
                            <property
                              containsID="true"
                              dataType="System.Int32"
                              description="Output column lineage ID"
                              name="OutputColumnLineageID">#{Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[cDealable]}</property>
                          </properties>
                        </inputColumn>
                      </inputColumns>
                      <externalMetadataColumns />
                    </input>
                    <input
                      refId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 4]"
                      dangling="true"
                      hasSideEffects="true"
                      name="Union All Input 4">
                      <externalMetadataColumns />
                    </input>
                  </inputs>
                  <outputs>
                    <output
                      refId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1]"
                      name="Union All Output 1">
                      <outputColumns>
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[lTid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[lTid]"
                          name="lTid" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[CurrencyPair]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[CurrencyPair]"
                          name="CurrencyPair" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateDateTime]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateDateTime]"
                          name="RateDateTime" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateBid]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateBid]"
                          name="RateBid" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateAsk]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[RateAsk]"
                          name="RateAsk" />
                        <outputColumn
                          refId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[cDealable]"
                          codePage="1252"
                          dataType="str"
                          length="50"
                          lineageId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1].Columns[cDealable]"
                          name="cDealable" />
                      </outputColumns>
                      <externalMetadataColumns />
                    </output>
                  </outputs>
                </component>
              </components>
              <paths>
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Data Conversion Error Output]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Data Error.Inputs[Flat File Destination Input]"
                  name="Data Conversion Error Output"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Error Output]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Data Conversion Output]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Inputs[Derived Column Input]"
                  name="Data Conversion Output"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Outputs[Data Conversion Output]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Derived Column Output]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Multicast.Inputs[Multicast Input 1]"
                  name="Derived Column Output"
                  startId="Package\Foreach Loop Container\Data Flow Task\Derived Column.Outputs[Derived Column Output]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[EMPTY_STRING]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 3]"
                  name="EMPTY_STRING"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[EMPTY_STRING]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Flat File Source Output]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Sort.Inputs[Sort Input]"
                  name="Flat File Source Output"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data Source.Outputs[Flat File Source Output]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Multicast Output 2]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Total Data Destination.Inputs[Flat File Destination Input]"
                  name="Multicast Output 2"
                  startId="Package\Foreach Loop Container\Data Flow Task\Multicast.Outputs[Multicast Output 2]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[NOTNULL_VALUE]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Inputs[Conditional Split Input]"
                  name="NOTNULL_VALUE"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[NOTNULL_VALUE]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[NOT_EMPTY_STRING]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Data Conversion.Inputs[Data Conversion Input]"
                  name="NOT_EMPTY_STRING"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Outputs[NOT_EMPTY_STRING]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[NOT_NULL_STRING]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING.Inputs[Conditional Split Input]"
                  name="NOT_NULL_STRING"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[NOT_NULL_STRING]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[NULL_STRING]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 2]"
                  name="NULL_STRING"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING.Outputs[NULL_STRING]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[NULL_VALUE]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Union All.Inputs[Union All Input 1]"
                  name="NULL_VALUE"
                  startId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Outputs[NULL_VALUE]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Sort Output]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE.Inputs[Conditional Split Input]"
                  name="Sort Output"
                  startId="Package\Foreach Loop Container\Data Flow Task\Sort.Outputs[Sort Output]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Total]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Data Destination.Inputs[Flat File Destination Input]"
                  name="Total"
                  startId="Package\Foreach Loop Container\Data Flow Task\Multicast.Outputs[Total]" />
                <path
                  refId="Package\Foreach Loop Container\Data Flow Task.Paths[Union All Output 1]"
                  endId="Package\Foreach Loop Container\Data Flow Task\Data NULL.Inputs[Flat File Destination Input]"
                  name="Union All Output 1"
                  startId="Package\Foreach Loop Container\Data Flow Task\Union All.Outputs[Union All Output 1]" />
              </paths>
            </pipeline>
          </DTS:ObjectData>
        </DTS:Executable>
      </DTS:Executables>
      <DTS:ForEachVariableMappings>
        <DTS:ForEachVariableMapping
          DTS:CreationName=""
          DTS:DTSID="{B853E7A1-157C-465D-87D3-A6BBC9FC3262}"
          DTS:ObjectName="{B853E7A1-157C-465D-87D3-A6BBC9FC3262}"
          DTS:ValueIndex="0"
          DTS:VariableName="User::Variable" />
      </DTS:ForEachVariableMappings>
    </DTS:Executable>
  </DTS:Executables>
  <DTS:PrecedenceConstraints>
    <DTS:PrecedenceConstraint
      DTS:refId="Package.PrecedenceConstraints[Constraint]"
      DTS:CreationName=""
      DTS:DTSID="{D42A26E3-5CEF-4243-B936-BCA9A377D173}"
      DTS:From="Package\Foreach Loop Container"
      DTS:LogicalAnd="True"
      DTS:ObjectName="Constraint"
      DTS:To="Package\Data Flow Task" />
  </DTS:PrecedenceConstraints>
  <DTS:DesignTimeProperties><![CDATA[<?xml version="1.0"?>
<!--This CDATA section contains the layout information of the package. The section includes information such as (x,y) coordinates, width, and height.-->
<!--If you manually edit this section and make a mistake, you can delete it. -->
<!--The package will still be able to load normally but the previous layout information will be lost and the designer will automatically re-arrange the elements on the design surface.-->
<Objects
  Version="8">
  <!--Each node below will contain properties that do not affect runtime behavior.-->
  <Package
    design-time-name="Package">
    <LayoutInfo>
      <GraphLayout
        Capacity="4" xmlns="clr-namespace:Microsoft.SqlServer.IntegrationServices.Designer.Model.Serialization;assembly=Microsoft.SqlServer.IntegrationServices.Graph" xmlns:mssgle="clr-namespace:Microsoft.SqlServer.Graph.LayoutEngine;assembly=Microsoft.SqlServer.Graph" xmlns:assembly="http://schemas.microsoft.com/winfx/2006/xaml">
        <NodeLayout
          Size="151,42"
          Id="Package\Foreach Loop Container\Data Flow Task"
          TopLeft="46,31" />
        <ContainerLayout
          HeaderHeight="43"
          IsExpanded="True"
          PanelSize="240,128"
          Size="240,171"
          Id="Package\Foreach Loop Container"
          TopLeft="270,48" />
        <NodeLayout
          Size="151,42"
          Id="Package\Data Flow Task"
          TopLeft="613,118" />
        <EdgeLayout
          Id="Package.PrecedenceConstraints[Constraint]"
          TopLeft="510,136.25">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="103,0"
              Start="0,0"
              End="95.5,0">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="95.5,0" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
      </GraphLayout>
    </LayoutInfo>
  </Package>
  <TaskHost
    design-time-name="Package\Foreach Loop Container\Data Flow Task">
    <LayoutInfo>
      <GraphLayout
        Capacity="32" xmlns="clr-namespace:Microsoft.SqlServer.IntegrationServices.Designer.Model.Serialization;assembly=Microsoft.SqlServer.IntegrationServices.Graph" xmlns:mssgle="clr-namespace:Microsoft.SqlServer.Graph.LayoutEngine;assembly=Microsoft.SqlServer.Graph" xmlns:assembly="http://schemas.microsoft.com/winfx/2006/xaml" xmlns:mssgm="clr-namespace:Microsoft.SqlServer.Graph.Model;assembly=Microsoft.SqlServer.Graph">
        <NodeLayout
          Size="98,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Sort"
          TopLeft="341,102" />
        <NodeLayout
          Size="136,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data Source"
          TopLeft="319,22" />
        <NodeLayout
          Size="184,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Total Data Destination"
          TopLeft="470.166666666667,970.333333333333" />
        <NodeLayout
          Size="128,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data Error"
          TopLeft="77.5,648.333333333333" />
        <NodeLayout
          Size="157,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data Destination"
          TopLeft="224.5,974.833333333333" />
        <NodeLayout
          Size="120,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Multicast"
          TopLeft="351.166666666667,800.333333333333" />
        <NodeLayout
          Size="169,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data NULL STRING"
          TopLeft="302,299" />
        <NodeLayout
          Size="163,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data NULL VALUE"
          TopLeft="310,189" />
        <NodeLayout
          Size="121,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Union All"
          TopLeft="620.333333333333,430.166666666667" />
        <NodeLayout
          Size="129,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data NULL"
          TopLeft="617.833333333333,638.666666666667" />
        <NodeLayout
          Size="177,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data EMPTY STRING"
          TopLeft="302.5,430.833333333333" />
        <NodeLayout
          Size="156,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Data Conversion"
          TopLeft="318.333333333333,530.833333333333" />
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Union All Output 1]"
          TopLeft="681.583333333333,472.166666666667">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,166.5"
              Start="0,0"
              End="0,159">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,159" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Total]"
          TopLeft="392.5,842.333333333333">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="-89.5000000000003,132.5"
              Start="0,0"
              End="-89.5000000000003,125">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,50.0460526315789" />
                  <mssgle:CubicBezierSegment
                    Point1="0,50.0460526315789"
                    Point2="0,54.0460526315789"
                    Point3="-4,54.0460526315789" />
                  <mssgle:LineSegment
                    End="-85.5000000000003,54.0460526315789" />
                  <mssgle:CubicBezierSegment
                    Point1="-85.5000000000003,54.0460526315789"
                    Point2="-89.5000000000003,54.0460526315789"
                    Point3="-89.5000000000003,58.0460526315789" />
                  <mssgle:LineSegment
                    End="-89.5000000000003,125" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Sort Output]"
          TopLeft="390.75,144">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,45"
              Start="0,0"
              End="0,37.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,37.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[NULL_VALUE]"
          TopLeft="412.6,231">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="287.066666666667,199.166666666667"
              Start="0,0"
              End="287.066666666667,191.666666666667">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,22.67108159611" />
                  <mssgle:CubicBezierSegment
                    Point1="0,22.67108159611"
                    Point2="0,26.67108159611"
                    Point3="4,26.67108159611" />
                  <mssgle:LineSegment
                    End="283.066666666667,26.67108159611" />
                  <mssgle:CubicBezierSegment
                    Point1="283.066666666667,26.67108159611"
                    Point2="287.066666666667,26.67108159611"
                    Point3="287.066666666667,30.67108159611" />
                  <mssgle:LineSegment
                    End="287.066666666667,191.666666666667" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <mssgm:EdgeLabel
              BoundingBox="114.180384114583,31.67108159611,58.7058984375,10.7353515625"
              RelativePosition="Any" />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[NULL_STRING]"
          TopLeft="413.333333333333,341">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="248.666666666667,89.1666666666666"
              Start="0,0"
              End="248.666666666667,81.6666666666666">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,40.3798048726362" />
                  <mssgle:CubicBezierSegment
                    Point1="0,40.3798048726362"
                    Point2="0,44.3798048726362"
                    Point3="4,44.3798048726362" />
                  <mssgle:LineSegment
                    End="244.666666666667,44.3798048726362" />
                  <mssgle:CubicBezierSegment
                    Point1="244.666666666667,44.3798048726362"
                    Point2="248.666666666667,44.3798048726362"
                    Point3="248.666666666667,48.3798048726362" />
                  <mssgle:LineSegment
                    End="248.666666666667,81.6666666666666" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <mssgm:EdgeLabel
              BoundingBox="92.2688411458333,49.3798048726362,64.128984375,10.8671875"
              RelativePosition="Any" />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[NOT_NULL_STRING]"
          TopLeft="388.75,341">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,89.8333333333333"
              Start="0,0"
              End="0,82.3333333333333">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,82.3333333333333" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <mssgm:EdgeLabel
              BoundingBox="-44.5894921875,35.7233072916667,89.178984375,10.88671875"
              RelativePosition="Any" />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[NOT_EMPTY_STRING]"
          TopLeft="393.666666666667,472.833333333333">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,58.0000000000001"
              Start="0,0"
              End="0,50.5000000000001">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,50.5000000000001" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <mssgm:EdgeLabel
              BoundingBox="-48.2094921875,19.8066406250001,96.418984375,10.88671875"
              RelativePosition="Any" />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[NOTNULL_VALUE]"
          TopLeft="387.083333333333,231">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,68"
              Start="0,0"
              End="0,60.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,60.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <mssgm:EdgeLabel
              BoundingBox="-39.14794921875,24.806640625,78.2958984375,10.88671875"
              RelativePosition="Any" />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Multicast Output 2]"
          TopLeft="429.833333333334,842.333333333333">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="132.333333333333,128"
              Start="0,0"
              End="132.333333333333,120.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,48.2105263157895" />
                  <mssgle:CubicBezierSegment
                    Point1="0,48.2105263157895"
                    Point2="0,52.2105263157895"
                    Point3="4,52.2105263157895" />
                  <mssgle:LineSegment
                    End="128.333333333333,52.2105263157895" />
                  <mssgle:CubicBezierSegment
                    Point1="128.333333333333,52.2105263157895"
                    Point2="132.333333333333,52.2105263157895"
                    Point3="132.333333333333,56.2105263157895" />
                  <mssgle:LineSegment
                    End="132.333333333333,120.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Flat File Source Output]"
          TopLeft="388.5,64">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,38"
              Start="0,0"
              End="0,30.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,30.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[EMPTY_STRING]"
          TopLeft="479.5,451.5">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="140.833333333333,0"
              Start="0,0"
              End="133.333333333333,0">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="133.333333333333,0" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <mssgm:EdgeLabel
              BoundingBox="30.9821744791667,5,71.368984375,10.8671875"
              RelativePosition="Any" />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Data Conversion Error Output]"
          TopLeft="371.666666666667,572.833333333333">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="-230.166666666667,75.5"
              Start="0,0"
              End="-230.166666666667,68">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,26.6598984771574" />
                  <mssgle:CubicBezierSegment
                    Point1="0,26.6598984771574"
                    Point2="0,30.6598984771574"
                    Point3="-4,30.6598984771574" />
                  <mssgle:LineSegment
                    End="-226.166666666667,30.6598984771574" />
                  <mssgle:CubicBezierSegment
                    Point1="-226.166666666667,30.6598984771574"
                    Point2="-230.166666666667,30.6598984771574"
                    Point3="-230.166666666667,34.6598984771574" />
                  <mssgle:LineSegment
                    End="-230.166666666667,68" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <mssgm:EdgeLabel
              BoundingBox="-181.169720052083,35.6598984771574,132.1727734375,11.43359375"
              RelativePosition="Any" />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <NodeLayout
          Size="154,42"
          Id="Package\Foreach Loop Container\Data Flow Task\Derived Column"
          TopLeft="329,660" />
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Data Conversion Output]"
          TopLeft="406,572.833333333333">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,87.166666666667"
              Start="0,0"
              End="0,79.666666666667">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,79.666666666667" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Foreach Loop Container\Data Flow Task.Paths[Derived Column Output]"
          TopLeft="408.583333333333,702">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,98.333333333333"
              Start="0,0"
              End="0,90.833333333333">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,90.833333333333" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
      </GraphLayout>
    </LayoutInfo>
  </TaskHost>
  <TaskHost
    design-time-name="Package\Data Flow Task">
    <LayoutInfo>
      <GraphLayout
        Capacity="32" xmlns="clr-namespace:Microsoft.SqlServer.IntegrationServices.Designer.Model.Serialization;assembly=Microsoft.SqlServer.IntegrationServices.Graph" xmlns:mssgle="clr-namespace:Microsoft.SqlServer.Graph.LayoutEngine;assembly=Microsoft.SqlServer.Graph" xmlns:assembly="http://schemas.microsoft.com/winfx/2006/xaml">
        <NodeLayout
          Size="151,42"
          Id="Package\Data Flow Task\Flat File Source"
          TopLeft="423,20" />
        <NodeLayout
          Size="190,42"
          Id="Package\Data Flow Task\Data Destination Yearly"
          TopLeft="458,685" />
        <NodeLayout
          Size="156,42"
          Id="Package\Data Flow Task\Data Conversion"
          TopLeft="422,128" />
        <NodeLayout
          Size="154,42"
          Id="Package\Data Flow Task\Derived Column"
          TopLeft="425,227" />
        <NodeLayout
          Size="133,42"
          Id="Package\Data Flow Task\Data Yearly"
          TopLeft="455,463" />
        <NodeLayout
          Size="120,42"
          Id="Package\Data Flow Task\Multicast"
          TopLeft="444,335" />
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Derived Column Output]"
          TopLeft="503,269">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,66"
              Start="0,0"
              End="0,58.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,58.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Multicast Output 1]"
          TopLeft="522.083333333333,377">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,86"
              Start="0,0"
              End="0,78.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,78.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Data Conversion Output]"
          TopLeft="501,170">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,57"
              Start="0,0"
              End="0,49.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,49.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <NodeLayout
          Size="142,42"
          Id="Package\Data Flow Task\Data Monthly"
          TopLeft="294,463" />
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Multicast Output 2]"
          TopLeft="485.333333333333,377">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="-120.333333333333,86"
              Start="0,0"
              End="-120.333333333333,78.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,31.078947368421" />
                  <mssgle:CubicBezierSegment
                    Point1="0,31.078947368421"
                    Point2="0,35.078947368421"
                    Point3="-4,35.078947368421" />
                  <mssgle:LineSegment
                    End="-116.333333333333,35.078947368421" />
                  <mssgle:CubicBezierSegment
                    Point1="-116.333333333333,35.078947368421"
                    Point2="-120.333333333333,35.078947368421"
                    Point3="-120.333333333333,39.078947368421" />
                  <mssgle:LineSegment
                    End="-120.333333333333,78.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <NodeLayout
          Size="198,42"
          Id="Package\Data Flow Task\Data Destination Monthly"
          TopLeft="259,688" />
        <NodeLayout
          Size="139,42"
          Id="Package\Data Flow Task\Sort Monthly"
          TopLeft="289,581" />
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Aggregate Output 1]"
          TopLeft="361.75,505">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,76"
              Start="0,0"
              End="0,68.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,68.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Sort Output]"
          TopLeft="358.25,623">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,65"
              Start="0,0"
              End="0,57.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,57.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <NodeLayout
          Size="130,42"
          Id="Package\Data Flow Task\Sort Yearly"
          TopLeft="463,583" />
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Aggregate Output 11]"
          TopLeft="524.75,505">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,78"
              Start="0,0"
              End="0,70.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,70.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Sort Output1]"
          TopLeft="528.5,625">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,60"
              Start="0,0"
              End="0,52.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,52.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Flat File Source Output]"
          TopLeft="499.25,62">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,66"
              Start="0,0"
              End="0,58.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,58.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <NodeLayout
          Size="127,42"
          Id="Package\Data Flow Task\Data Daily"
          TopLeft="630,466" />
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Multicast Output 3]"
          TopLeft="532,377">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="161.5,89"
              Start="0,0"
              End="161.5,81.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,26.9565217391304" />
                  <mssgle:CubicBezierSegment
                    Point1="0,26.9565217391304"
                    Point2="0,30.9565217391304"
                    Point3="4,30.9565217391304" />
                  <mssgle:LineSegment
                    End="157.5,30.9565217391304" />
                  <mssgle:CubicBezierSegment
                    Point1="157.5,30.9565217391304"
                    Point2="161.5,30.9565217391304"
                    Point3="161.5,34.9565217391304" />
                  <mssgle:LineSegment
                    End="161.5,81.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <NodeLayout
          Size="125,42"
          Id="Package\Data Flow Task\Sort Daily"
          TopLeft="642,582" />
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Aggregate Output 12]"
          TopLeft="705.5,508">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="0,74"
              Start="0,0"
              End="0,66.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,66.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
        <NodeLayout
          Size="184,42"
          Id="Package\Data Flow Task\Data Destination Daily"
          TopLeft="651,686" />
        <EdgeLayout
          Id="Package\Data Flow Task.Paths[Sort Output2]"
          TopLeft="704.5,624">
          <EdgeLayout.Curve>
            <mssgle:Curve
              StartConnector="{assembly:Null}"
              EndConnector="38.5,62"
              Start="0,0"
              End="38.5,54.5">
              <mssgle:Curve.Segments>
                <mssgle:SegmentCollection
                  Capacity="5">
                  <mssgle:LineSegment
                    End="0,27" />
                  <mssgle:CubicBezierSegment
                    Point1="0,27"
                    Point2="0,31"
                    Point3="4,31" />
                  <mssgle:LineSegment
                    End="34.5,31" />
                  <mssgle:CubicBezierSegment
                    Point1="34.5,31"
                    Point2="38.5,31"
                    Point3="38.5,35" />
                  <mssgle:LineSegment
                    End="38.5,54.5" />
                </mssgle:SegmentCollection>
              </mssgle:Curve.Segments>
            </mssgle:Curve>
          </EdgeLayout.Curve>
          <EdgeLayout.Labels>
            <EdgeLabelCollection />
          </EdgeLayout.Labels>
        </EdgeLayout>
      </GraphLayout>
    </LayoutInfo>
  </TaskHost>
</Objects>]]></DTS:DesignTimeProperties>
</DTS:Executable>
