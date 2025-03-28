# CAP LLM Plugin

CAP LLM Plugin helps developers create tailored Generative AI based CAP applications:

1. Without exposing confidential data to LLM by anonymizing sensitive data leveraging SAP HANA Cloud Data Anonymization.
2. Seamlessly generate vector embeddings via SAP AI Core.
3. Easily retrieve Chat Completion response via SAP AI Core.
4. Efforlessly perform similarity search via SAP HANA Cloud Vector engine.
5. Simplified single RAG (retrieval-augmented generation) retrieval method powered by SAP AI Core and SAP HANA Cloud Vector Engine.

## ✔️ Anonymization Features


|                         **Feature**                                                           |                                                           **Details**    
| :-------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------
|  Seamlessly anonymize sensitive data using a variety of SAP HANA Cloud's anonymization capabilities |   Effortlessly anonymize sensitive data within a CAP application by employing a single `@anonymize` annotation using a diverse range of SAP HANA Cloud's anonymization algorithms, including but not limited to: <li> [k-Anonymity](https://help.sap.com/docs/SAP_HANA_PLATFORM/f88e51df089949b2af06ac891c77abf8/205f52e73c4a422e91fb9a0fbd5f3ec6.html)</li><li> [l-Diversity](https://help.sap.com/docs/SAP_HANA_PLATFORM/f88e51df089949b2af06ac891c77abf8/eeb681e53a06434ca8a0fd20ab9c2b7c.html)</li><li> [Differential Privacy](https://help.sap.com/docs/SAP_HANA_PLATFORM/f88e51df089949b2af06ac891c77abf8/ace3f36bad754cc9bbfe2bf473fccf2f.html)</li></ul>|
| Effortlessly replace the anonymized data within the LLM response with  genuine information|  Given that the data provided to the LLM consists of anonymized information, the CAP LLM plugin ensures a seamless replacement of anonymized content within the LLM response with the corresponding authentic data.    

## 🎯 LLM Access Layer Features

|                         **Feature**                                                           |                                                           **Details**    
| :-------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------
|  Embedding generation via SAP AI Core | Easily connect to embedding models via SAP AI Core and generate embeddings seamlessly |
|  Similarity search  |  Leverage the SAP HANA Cloud's Vector engine to perform similarity search via CAP LLM Plugin |  
|  Chat LLM Access via SAP AI Core |   Simple access to LLM models via SAP AI Core with simplified method for chat completion |  
|  Streamlining RAG retrieval  |   Single method to streamline the entire RAG retrieval process leveraging SAP AI Core and SAP HANA Cloud Vector Engine |



## 📚 Samples and documentation

For API documentation of CAP LLM Plugin, check the doc folder under the Code tab of this page or go to SAP Samples as mentioned below.

For sample use cases leveraging CAP LLM Plugin, refer to [SAP Samples](https://github.com/SAP-samples/cap-llm-plugin-samples).


## ❗ Version Upgrade Notice
From 1.3.* to 1.4.2 (function signature changed for following methods, version not recommended):   
getEmbedding  
getChatCompletion  
getRagResponse  

From 1.3.* to 1.4.4 and above(backwards compatible, new methods to support more models):   
No change required unless you want to use new methods supporting new models as mentioned in API document:  
(old)getEmbedding -> getEmbeddingWithConfig  
(old)getChatCompletion -> getChatCompletionWithConfig  
(old)getRagResponse -> getRagResponseWithConfig  

## 🙌 Support and Contact

This project is provided "as-is" with no expectation for major changes or support.
