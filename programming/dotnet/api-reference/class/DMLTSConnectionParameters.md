---
layout: default-layout
title: Dynamsoft Barcode Reader .NET API Reference - DMLTSConnectionParameters Class
description: This page shows the DMLTSConnectionParameters Class of Dynamsoft Barcode Reader for .NET SDK.
keywords: DMLTSConnectionParameters, class, api reference, .Net
needAutoGenerateSidebar: false
---


# DMLTSConnectionParameters

Defines a struct to configure the parameters to connect to license tracking server.  

```C#
public class DMLTSConnectionParameters
```  

---

## Attributes
    
| Attribute | Type |
|---------- | ---- |
| [`MainServerURL`](#mainserverurl) | *string* |
| [`StandbyServerURL`](#standbyserverurl) | *string* |
| [`HandshakeCode`](#handshakecode) | *string* |
| [`SessionPassword`](#sessionpassword) | *string* |
| [`DeploymentType`](#deploymenttype) | *EnumDMDeploymentType* |
| [`ChargeWay`](#chargeway) | *EnumDMChargeWay* |
| [`UUIDGenerationMethod`](#uuidgenerationmethod) | *EnumDMUUIDGenerationMethod* |
| [`MaxBufferDays`](#maxbufferdays) | *int* |
| [`LimitedLicenseModules`](#limitedlicensemodules) | *EnumDMLicenseModule[]* |


### MainServerURL

The URL of the license tracking server.

```C#
string Dynamsoft.Barcode.DMLTSConnectionParameters.MainServerURL
```

- **Value range**   
    Any string value   
      
- **Default value**   
    null

### StandbyServerURL

The URL of the standby license tracking server.

```C#
string Dynamsoft.Barcode.DMLTSConnectionParameters.StandbyServerURL
```

- **Value range**   
    Any string value   
      
- **Default value**   
    null

### HandshakeCode

The handshake code.

```C#
string Dynamsoft.Barcode.DMLTSConnectionParameters.HandshakeCode
```

- **Value range**   
    Any string value   
      
- **Default value**   
    null

### SessionPassword

The session password of the handshake code set in license tracking server.

```C#
string Dynamsoft.Barcode.DMLTSConnectionParameters.SessionPassword
```

- **Value range**   
    Any string value   
      
- **Default value**   
    null


### DeploymentType

Sets the deployment type.

```C#
EnumDMDeploymentType Dynamsoft.Barcode.DMLTSConnectionParameters.DeploymentType
```

- **Value range**   
    Any one of the [`EnumDMDeploymentType`]({{ site.enumerations }}other-enums.html#dm_deploymenttype) Enumeration items.   
      
- **Default value**   
    DM_DT_DESKTOP   
    
- **See also**  
    [`EnumDMDeploymentType`]({{ site.enumerations }}other-enums.html#dm_deploymenttype)    

### ChargeWay

Sets the charge way.

```C#
EnumDMChargeWay Dynamsoft.Barcode.DMLTSConnectionParameters.ChargeWay
```

- **Value range**   
    Any one of the [`EnumDMChargeWay`]({{ site.enumerations }}other-enums.html#dm_chargeWay) Enumeration items.   
      
- **Default value**   
    DM_CW_AUTO   
    
- **See also**  
    [`EnumDMChargeWay`]({{ site.enumerations }}other-enums.html#dm_chargeWay)    


### UUIDGenerationMethod

Sets the method to generate UUID.

```C#
EnumDMUUIDGenerationMethod Dynamsoft.Barcode.DMLTSConnectionParameters.UUIDGenerationMethod
```

- **Value range**   
    Any one of the [`EnumDMUUIDGenerationMethod`]({{ site.enumerations }}other-enums.html#dm_uuidgenerationmethod) Enumeration items.   
      
- **Default value**   
    DM_UUIDGM_RANDOM   
    
- **See also**  
    [`EnumDMUUIDGenerationMethod`]({{ site.enumerations }}other-enums.html#dm_uuidgenerationmethod)    

### MaxBufferDays

Sets the max days to buffer the license info.

```C#
int Dynamsoft.Barcode.DMLTSConnectionParameters.MaxBufferDays
```

- **Value range**   
    [0,0x7fffffff]  
      
- **Default value**   
    0   
    

### LimitedLicenseModules

Sets the license modules to use.

```C#
EnumDMLicenseModule[] Dynamsoft.Barcode.DMLTSConnectionParameters.LimitedLicenseModules
```

- **Value range**   
    Each array item can be any one of the [`EnumDMLicenseModule`]({{ site.enumerations }}other-enums.html#dm_licensemodule) Enumeration items.   
      
- **Default value**   
    null   
    
- **See also**  
    [`EnumDMLicenseModule`]({{ site.enumerations }}other-enums.html#dm_licensemodule)    
