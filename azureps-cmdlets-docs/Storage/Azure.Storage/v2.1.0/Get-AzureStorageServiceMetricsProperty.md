---
external help file: Microsoft.WindowsAzure.Commands.Storage.dll-Help.xml
online version: .\New-AzureStorageContext.md
schema: 2.0.0
ms.assetid: 59B6D8FB-70FF-4B9E-B6AF-E303E1451DBB
---

# Get-AzureStorageServiceMetricsProperty

## SYNOPSIS
Gets metrics properties for the Azure Storage service.

## SYNTAX

```
Get-AzureStorageServiceMetricsProperty [-ServiceType] <StorageServiceType> [-MetricsType] <ServiceMetricsType>
 [-Context <AzureStorageContext>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureStorageServiceMetricsProperty** cmdlet gets metrics properties for the Azure Storage service.

## EXAMPLES

### Example 1: Get metrics properties for the Blob service
```
C:\PS>Get-AzureStorageServiceMetricsProperty -ServiceType Blob -MetricsType Hour
```

This command gets metrics properties for blob storage for the Hour metrics type.

## PARAMETERS

### -ServiceType
Specifies the storage service type.
This cmdlet gets the metrics properties for the type that this parameter specifies.
The acceptable values for this parameter are:

- Blob 
- Table
- Queue
- File 

The value of File is not currently supported.

```yaml
Type: StorageServiceType
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MetricsType
Specifies a metrics type.
This cmdlet gets the Azure Storage service metrics properties for the metrics type that this parameter specifies.
The acceptable values for this parameter are: Hour and Minute.

```yaml
Type: ServiceMetricsType
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Context
Specifies an Azure storage context.
To obtain a storage context, use the New-AzureStorageContext cmdlet.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PipelineVariable
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureStorageContext](.\New-AzureStorageContext.md)

[Set-AzureStorageServiceMetricsProperty](.\Set-AzureStorageServiceMetricsProperty.md)


