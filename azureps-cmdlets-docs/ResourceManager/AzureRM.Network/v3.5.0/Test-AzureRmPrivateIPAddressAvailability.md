---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 0780CB09-9C3B-468A-A718-3A646FE3D152
online version:
schema: 2.0.0
content_git_url: https://github.com/Visual-Studio-China/azure-powershell/blob/3.6.0/src/ResourceManager/Network/Commands.Network/help/Test-AzureRmPrivateIPAddressAvailability.md
original_content_git_url: https://github.com/Visual-Studio-China/azure-powershell/blob/3.6.0/src/ResourceManager/Network/Commands.Network/help/Test-AzureRmPrivateIPAddressAvailability.md
gitcommit: https://github.com/Visual-Studio-China/azure-powershell/blob/94e42834e29c78cafba9e3f1e99e14af92561036
---

# Test-AzureRmPrivateIPAddressAvailability

## SYNOPSIS
Test availability of a private IP address in a virtual network.

## SYNTAX

### TestByResource
```
Test-AzureRmPrivateIPAddressAvailability -VirtualNetwork <PSVirtualNetwork> -IPAddress <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### TestByResourceId
```
Test-AzureRmPrivateIPAddressAvailability -ResourceGroupName <String> -VirtualNetworkName <String>
 -IPAddress <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Test-AzureRmPrivateIPAddressAvailability** cmdlet tests whether a specified private IP address is available in a virtual network.
This cmdlet returns a list of available private IP addresses if the requested private IP address is taken.

## EXAMPLES

### Example 1: Test whether an IP address is available using the pipeline
```
PS C:\>Get-AzureRmVirtualNetwork -Name $vnetName -ResourceGroupName $rgname | Test-AzureRmPrivateIPAddressAvailability -IPAddress "10.0.1.10"
```

This command gets a virtual network and uses the pipeline operator to pass it to **Test-AzureRmPrivateIPAddressAvailability**, which tests whether the specified private IP address is available.

## PARAMETERS

### -VirtualNetwork
Specifies a **PSVirtualNetwork** object.

```yaml
Type: PSVirtualNetwork
Parameter Sets: TestByResource
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IPAddress
Specifies the IP address to test.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
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
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group for the virtual network.

```yaml
Type: String
Parameter Sets: TestByResourceId
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VirtualNetworkName
Specifies the name of the virtual network.

```yaml
Type: String
Parameter Sets: TestByResourceId
Aliases: 

Required: True
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

[Get-AzureRmVirtualNetwork](./Get-AzureRmVirtualNetwork.md)


