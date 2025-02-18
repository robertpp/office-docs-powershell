---
external help file: Microsoft.Exchange.TransportMailflow-Help.xml
online version: https://docs.microsoft.com/powershell/module/exchange/get-adaptivescope
applicable: Security & Compliance
title: Get-AdaptiveScope
schema: 2.0.0
author: chrisda
ms.author: chrisda
ms.reviewer:
---

# Get-AdaptiveScope

## SYNOPSIS
This cmdlet is available only in Security & Compliance PowerShell. For more information, see [Security & Compliance PowerShell](https://docs.microsoft.com/powershell/exchange/scc-powershell).

Use the Get-AdaptiveScope cmdlet to view adaptive scopes in your organization. Adaptive scopes (or static scopes) are used in retention policies and retention label policies.

For information about the parameter sets in the Syntax section below, see [Exchange cmdlet syntax](https://docs.microsoft.com/powershell/exchange/exchange-cmdlet-syntax).

## SYNTAX

```
Get-AdaptiveScope [[-Identity] <ComplianceRuleIdParameter>] [<CommonParameters>]
```

## DESCRIPTION
To use this cmdlet in Security & Compliance PowerShell, you need to be assigned permissions. For more information, see [Permissions in the Microsoft Purview compliance portal](https://docs.microsoft.com/microsoft-365/compliance/microsoft-365-compliance-center-permissions).

## EXAMPLES

### Example 1
```powershell
Get-AdaptiveScope | Format-Table Name,Priority
```

This example returns a summary list of all adaptive scopes.
### Example 2
```powershell
Get-AdaptiveScope -Identity "Project X"
```

This example returns detailed information about the adaptive scope named Project X.

## PARAMETERS

### -Identity
The Identity parameter specifies the adaptive scope that you want to view. You can use any value that uniquely identifies the adaptive scope. For example:

- Name
- Distinguished name (DN)
- GUID

```yaml
Type: ComplianceRuleIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Security & Compliance

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
