# Revision history for ollama-haskell

## Unreleased

## 0.2.0.0 -- 2025-06-05

* Added stack matrix to ensure lib is buildable from lts-19.33
* Made parameters & template fields optional in `ShowModelResponse`.
* Added extra parameters fields in `ModelInfo`.
* Added strict annotations for all fields.
* Fixed ToJSON instance for delete model request body.
* Removed duplicate code by using unified `withOllamaRequest` function for all API calls.
* Added unified config type `OllamaConfig` to hold common configuration options.
* Added validation for generate and chat functions to ensure required fields are present.
* Added convience functions for generating Message and ToolCall types.
* Added thinking field for chat and generate function.
* Added ModelOptions type to encapsulate model options.
* Added get ollama version function.
* Added Common Manager, Callback functions and retry option in OllamaConfig.
* Fixed tool_calls.
* Added MonadIO versions of api functions.
* Added more comprehensive error handling for API calls.
* Added more comprehensive test cases for all functions.
* Added schema builder for passing json format for structured output.

## 0.1.3.0 -- 2025-03-25

* Added options, tools and tool_calls fields in chat and generate.
* Exported EmbeddingResponse.
* Added Format argument in chat and generate function for structured output.

## 0.1.2.0 -- 2024-11-20

* Added hostUrl and responseTimeOut options in generate function.
* Added hostUrl and responseTimeOut options in chat function.

## 0.1.1.3 -- 2024-11-08

* Increase response timeout to 15 minutes
* Added encodeImage utility function that converts image filePath to base64 image data.
* Added generateJson and chatJson. High level function to return response in Haskell type.

## 0.1.0.3 -- 2024-11-05

* Moving to stack instead of cabal.

## 0.1.0.2 -- 2024-10-18

* Increased response timeout time for chat function. 

## 0.1.0.1 -- 2024-10-18

* Renaming Lib.hs to OllamaExamples.hs as it was conflicting `Lib.hs` name

## 0.1.0.0 -- YYYY-mm-dd

* First version. Released on an unsuspecting world.
