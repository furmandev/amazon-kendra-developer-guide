--------

--------

# AttributeFilter<a name="API_AttributeFilter"></a>

Provides filtering the query results based on document attributes\.

When you use the `AndAllFilters` or `OrAllFilters`, filters you can use 2 layers under the first attribute filter\. For example, you can use:

 `<AndAllFilters>` 

1.  ` <OrAllFilters>` 

1.  ` <EqualTo>` 

If you use more than 2 layers, you receive a `ValidationException` exception with the message "`AttributeFilter` cannot have a depth of more than 2\."

If you use more than 10 attribute filters, you receive a `ValidationException` exception with the message "`AttributeFilter` cannot have a length of more than 10"\.

## Contents<a name="API_AttributeFilter_Contents"></a>

 ** AndAllFilters **   <a name="Kendra-Type-AttributeFilter-AndAllFilters"></a>
Performs a logical `AND` operation on all supplied filters\.  
Type: Array of [ AttributeFilter ](#API_AttributeFilter) objects  
Required: No

 ** ContainsAll **   <a name="Kendra-Type-AttributeFilter-ContainsAll"></a>
Returns true when a document contains all of the specified document attributes\. This filter is only applicable to `StringListValue` metadata\.  
Type: [ DocumentAttribute ](API_DocumentAttribute.md) object  
Required: No

 ** ContainsAny **   <a name="Kendra-Type-AttributeFilter-ContainsAny"></a>
Returns true when a document contains any of the specified document attributes\. This filter is only applicable to `StringListValue` metadata\.  
Type: [ DocumentAttribute ](API_DocumentAttribute.md) object  
Required: No

 ** EqualsTo **   <a name="Kendra-Type-AttributeFilter-EqualsTo"></a>
Performs an equals operation on two document attributes\.  
Type: [ DocumentAttribute ](API_DocumentAttribute.md) object  
Required: No

<<<<<<< HEAD
 ** GreaterThan **   <a name="Kendra-Type-AttributeFilter-GreaterThan"></a>
Performs a greater than operation on two document attributes\. Use with a document attribute of type `Date` or `Long`\.  
Type: [ DocumentAttribute ](API_DocumentAttribute.md) object  
Required: No

 ** GreaterThanOrEquals **   <a name="Kendra-Type-AttributeFilter-GreaterThanOrEquals"></a>
Performs a greater or equals than operation on two document attributes\. Use with a document attribute of type `Date` or `Long`\.  
Type: [ DocumentAttribute ](API_DocumentAttribute.md) object  
Required: No

 ** LessThan **   <a name="Kendra-Type-AttributeFilter-LessThan"></a>
Performs a less than operation on two document attributes\. Use with a document attribute of type `Date` or `Long`\.  
Type: [ DocumentAttribute ](API_DocumentAttribute.md) object  
Required: No

 ** LessThanOrEquals **   <a name="Kendra-Type-AttributeFilter-LessThanOrEquals"></a>
Performs a less than or equals operation on two document attributes\. Use with a document attribute of type `Date` or `Long`\.  
Type: [ DocumentAttribute ](API_DocumentAttribute.md) object  
=======
 **GreaterThan**   <a name="Kendra-Type-AttributeFilter-GreaterThan"></a>
Performs a greater than operation on two document attributes\. Use with a document attribute of type `Integer` or `Long`\.  
Type: [DocumentAttribute](API_DocumentAttribute.md) object  
Required: No

 **GreaterThanOrEquals**   <a name="Kendra-Type-AttributeFilter-GreaterThanOrEquals"></a>
Performs a greater or equals than operation on two document attributes\. Use with a document attribute of type `Integer` or `Long`\.  
Type: [DocumentAttribute](API_DocumentAttribute.md) object  
Required: No

 **LessThan**   <a name="Kendra-Type-AttributeFilter-LessThan"></a>
Performs a less than operation on two document attributes\. Use with a document attribute of type `Integer` or `Long`\.  
Type: [DocumentAttribute](API_DocumentAttribute.md) object  
Required: No

 **LessThanOrEquals**   <a name="Kendra-Type-AttributeFilter-LessThanOrEquals"></a>
Performs a less than or equals operation on two document attributes\. Use with a document attribute of type `Integer` or `Long`\.  
Type: [DocumentAttribute](API_DocumentAttribute.md) object  
>>>>>>> parent of 39aa2d1 (Documentation updates include new features: data source connectors Amazon WorkDocs, SharePoint Server, Web crawler, new capacity units, and new API updates)
Required: No

 ** NotFilter **   <a name="Kendra-Type-AttributeFilter-NotFilter"></a>
Performs a logical `NOT` operation on all supplied filters\.  
Type: [ AttributeFilter ](#API_AttributeFilter) object  
Required: No

 ** OrAllFilters **   <a name="Kendra-Type-AttributeFilter-OrAllFilters"></a>
Performs a logical `OR` operation on all supplied filters\.  
Type: Array of [ AttributeFilter ](#API_AttributeFilter) objects  
Required: No

## See Also<a name="API_AttributeFilter_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [ AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/kendra-2019-02-03/AttributeFilter) 
+  [ AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/kendra-2019-02-03/AttributeFilter) 
+  [ AWS SDK for Java V2](https://docs.aws.amazon.com/goto/SdkForJavaV2/kendra-2019-02-03/AttributeFilter) 
+  [ AWS SDK for Ruby V3](https://docs.aws.amazon.com/goto/SdkForRubyV3/kendra-2019-02-03/AttributeFilter) 