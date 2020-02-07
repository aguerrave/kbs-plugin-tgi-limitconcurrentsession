# KBS Plugin : TGI Limit Concurrent Session

The fork from https://bitbucket.org/nmicoud/org.tgi.limit-concurrent-session, and converted to be installed via **KBS ObjectData Tool** 

Please refer to [http://wiki.idempiere.org/en/Plugin:_Limit_Concurrent_Sessions](http://wiki.idempiere.org/en/Plugin:_Limit_Concurrent_Sessions)

## How to install

1. Install **KBS ObjectData Tool** (refer to http://wiki.idempiere.org/en/Plugin:_ObjectDataTool)

2. Install the plugin via Apache Felix Web Console

## How to use

* Clent Level
* Organization Level
* Role Level
* User Level

## Fixing

Re-zip 2Pack by below changes:

Replace wrong `<EntityType>U</EntityType>` by `<EntityType>TGI</EntityType>`

In 2Pack, some wrong AD data also link to this plugin, remove it manually while convert to KBS ODT plugin

Remove wrong <AD_Field>

```
	<AD_Field type="table">
        <AD_Client_ID>0</AD_Client_ID>
        <AD_Org_ID>0</AD_Org_ID>
        <AD_Column_ID reference="uuid" reference-key="AD_Column">9429e973-ad39-411a-8094-db728bcc3664</AD_Column_ID>
        <AD_FieldGroup_ID reference="id"/>
        <AD_Field_UU>f82ab4df-6f84-49e3-8dc5-37729685e262</AD_Field_UU>
        <AD_Reference_ID reference="id"/>
        <AD_Reference_Value_ID reference="id"/>
        <AD_Tab_ID reference="id">119</AD_Tab_ID>
        <AD_Val_Rule_ID reference="id"/>
        <ColumnSpan>2</ColumnSpan>
        <DefaultValue/>
        <Description>This role is enabled for mobile access</Description>
        <DisplayLength>1</DisplayLength>
        <DisplayLogic/>
        <EntityType>U</EntityType>
        <Help/>
        <Included_Tab_ID reference="id"/>
        <IsActive>true</IsActive>
        <IsAdvancedField>false</IsAdvancedField>
        <IsAllowCopy/>
        <IsAlwaysUpdateable/>
        <IsCentrallyMaintained>true</IsCentrallyMaintained>
        <IsDefaultFocus>false</IsDefaultFocus>
        <IsDisplayed>true</IsDisplayed>
        <IsDisplayedGrid>true</IsDisplayedGrid>
        <IsEncrypted>false</IsEncrypted>
        <IsFieldOnly>false</IsFieldOnly>
        <IsHeading>false</IsHeading>
        <IsMandatory/>
        <IsQuickEntry>false</IsQuickEntry>
        <IsReadOnly>false</IsReadOnly>
        <IsSameLine>false</IsSameLine>
        <IsToolbarButton/>
        <IsUpdateable/>
        <MandatoryLogic/>
        <Name>Enabled for mobile access</Name>
        <NumLines>1</NumLines>
        <ObscureType/>
        <ReadOnlyLogic/>
        <SeqNo>110</SeqNo>
        <SeqNoGrid>460</SeqNoGrid>
        <SortNo/>
        <XPosition>2</XPosition>
        <AD_Field_Trl type="translation">
            <Description>This role is enabled for mobile access</Description>
            <Help/>
            <Name>Enabled for mobile access</Name>
            <AD_Language>es_ES</AD_Language>
            <IsActive>true</IsActive>
            <IsTranslated>false</IsTranslated>
        </AD_Field_Trl>
        <AD_Field_Trl type="translation">
            <Description>Rôle sélectionnable pour l'accès en version mobile</Description>
            <Help/>
            <Name>Utilisable pour l'accès mobile</Name>
            <AD_Language>fr_FR</AD_Language>
            <IsActive>true</IsActive>
            <IsTranslated>true</IsTranslated>
        </AD_Field_Trl>
        <AD_Field_Trl type="translation">
            <Description>This role is enabled for mobile access</Description>
            <Help/>
            <Name>Enabled for mobile access</Name>
            <AD_Language>it_IT</AD_Language>
            <IsActive>true</IsActive>
            <IsTranslated>false</IsTranslated>
        </AD_Field_Trl>
    </AD_Field>
```