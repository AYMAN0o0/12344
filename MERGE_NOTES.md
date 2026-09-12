# Nawabi Dastarkhwan — Merged Android Studio Project

This project is the merged Android foundation created from:
1. The fresh `NAWABIFOODDELIVERY` Android Studio project.
2. The Android implementation contained in the supplied ZIP.

## What was merged
- Existing Compose/Firebase AI foundation from the fresh project.
- Menu, dish models and variants.
- Room offline database and menu repository.
- Cart and WhatsApp order flow.
- Petpooja integration boundary (deliberately does NOT fake a POS sync or fabricate an order ID).
- Android biometric API helper.
- Nawabi theme and restaurant/menu UI.
- Firebase AI assistant screen, adapted from the original Gemini sample.
- Current Firebase `google-services.json` was retained so the existing Firebase package configuration remains valid.

## Important
The current application ID remains `com.example.nawabifooddelivery` because the supplied Firebase configuration is registered for that package. Do not rename the package until a Firebase Android app is registered for the new package ID and a new `google-services.json` is supplied.

The release build currently uses the debug keystore only for local testing. Configure a private release keystore before Play Store publishing.

## Intentionally NOT marked as complete yet
- Voice ordering / speech recognition
- Full production admin console
- Secure admin password management
- Direct dish image upload/storage
- Real Petpooja API authentication/configuration
- Real backend order synchronization
- Production payment gateway
- Production delivery tracking
- Play Store signing

These are left for the next development phase so the merged foundation does not contain fake or non-functional controls.

## Open
Open this folder directly in Android Studio and allow Gradle sync to complete.
Then test:
- Menu loading
- Dish variants
- Cart
- WhatsApp order intent
- AI Assistant
- Biometric prompt when available
