# Cledev.OpenAI _(Beta)_
Unofficial .NET SDK for OpenAI with a [Blazor Server Playground](https://github.com/lucabriguglia/Cledev.OpenAI.Playground)

[![Main](https://github.com/lucabriguglia/Cledev.OpenAI/actions/workflows/main.yml/badge.svg)](https://github.com/lucabriguglia/Cledev.OpenAI/actions/workflows/main.yml)
[![Nuget Package](https://img.shields.io/badge/nuget-1.0.0-blue.svg)](https://www.nuget.org/packages/Cledev.OpenAI)

```
Install-Package Cledev.OpenAI
```

## API

- **Models**
  - List Models
  - Retrieve Model
- **Completions**
  - Create Completion
- **Chat**
  - Create Chat Completion
- **Edits**
  - Create Edit
- **Images**
  - Create Image
  - Create Image Edit
  - Create Image Variation
- **Embeddings**
  - Create Embeddings
- **Audio**
  - Create Transcription
  - Create Translation
- **Files**
  - List Files
  - Upload File
  - Delete File
  - Retrieve File
- **Fine-tunes**
  - Create Fine-tune
  - List Fine-tunes
  - Retrieve Fine-tune
  - Cancel Fine-tune
  - List Fine-tune Events
  - Delete Fine-tune Model
- **Moderations**
  - Create Moderation

## Configuration

### Option 1

```C#
services.AddOpenAIClient();
```

This option requires an appsettings.json file

```json
{
  "OpenAI": {
    "ApiKey": "YOUR_API_KEY",
    "Organization": "OUR_ORGANIZATION"
  }
}
```

### Option 2

```C#
services.AddOpenAIClient(options =>
{
     options.ApiKey = "YOUR_API_KEY";
     options.Organization = "YOUR_ORGANIZATION";
 });
```

## Usage

Inject `IOpenAIClient` interface into your service

Please, have a look at the [Blazor Server Playground](https://github.com/lucabriguglia/Cledev.OpenAI.Playground) for examples on how to use the client.
