# Home Assistant GPT Integration

## Overview
Home Assistant GPT is a custom GPT assistant that interfaces with the Home Assistant API, allowing you to control and query various home devices with ease. This integration leverages the power of GPT-4 to provide an intuitive and responsive experience for managing your home automation setup.

## Pre-requisites

- A ChatGPT Plus account
- Your Home Assistant instance must be web facing.

## Features
- **Device Control**: Interact with lights and automations.
- **Weather Updates**: Get summaries and recommendations based on the weather.
- **Customizable Entity List**: Tailor the GPT to your specific Home Assistant setup.

## Setup Instructions

1. **GPT Initialization**:
   - Create a new GPT named 'Home Assistant'.
   - Use the following prompt, updating it with your entity list: [Prompt Link](https://raw.githubusercontent.com/BobbyHirst/HomeAssistantGPT/main/Prompt.txt)

2. **Action Integration**:
   - Add Actions using the provided OpenAPI Spec. Ensure to replace the URL with your public address: [API Spec Link](https://raw.githubusercontent.com/BobbyHirst/HomeAssistantGPT/main/ActionSpec.json)

3. **Authentication**:
   - Add an API Bearer Token for authentication. This token should be a long-lived token generated from your user page in the Home Assistant API.

4. **Finalizing GPT Setup**:
   - In your GPT settings, turn off "Use conversation data in your GPT to improve our models" for privacy.
   - Test the setup in the preview.

5. **Publication**:
   - When ready, publish the GPT. It's recommended to set it as Private for security.

## Entity Interaction

- **Lights**: Control and set colors of light entities (e.g., `light.office_lights`).
- **Automations**: Trigger automations for various home activities (e.g., `automation.boost_main_heating`).
- **Weather**: Provide weather summaries and recommendations (e.g., `weather.met_office_brighton_racecourse_3_hourly`).

## Future Enhancements
- **Voice Control**: Integration with OpenAI's Whisper model for voice commands.
- **Expansion of Supported Devices**: Increasing the variety of controllable entities.
- **User Experience Improvements**: Continual refinements for smoother interactions.

## Contributing
Contributions are welcome! This project is in its early stages and open to ideas, improvements, and creative enhancements.

## Disclaimer
This integration is not officially affiliated with OpenAI or Home Assistant.

---

_“Hey HomeAssistant, can you please lock up and let me know if the windows are all closed?” Just the beginning of what's possible with Home Assistant GPT._

