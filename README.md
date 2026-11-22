<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-xai 1.4.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-xai.git", from: "1.4.0")
```

Products: `SwiftAIXAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# xAI (Grok) for Swift

`SwiftAIXAI` adds xAI (Grok) to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/xai` and supports text generation, image generation, transcription, speech, video generation and provider files.

Provider guide with models, options, streaming and errors:

- [xAI (Grok)](https://swiftaisdk.github.io/SwiftAISDK/providers/xai/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIXAI` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIXAI

let provider = try AIProviders.xAI(configuration: XAIProviderSettings())
```

By default the provider reads `XAI_API_KEY` from the environment; values set in `XAIProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-xai` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
