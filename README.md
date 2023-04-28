# HubSpot Portal Launcher

A simple Raycast extension that allows you to quickly launch and navigate to different objects in your HubSpot portals. This extension is perfect for people who are working on and/or maintaining multiple portals like HubSpot Partner employees and developers. If you're using only one portal, I recommend using the [HubSpot Raycast Extension](https://www.raycast.com/harisvsulaiman/hubspot) by [Haris Sulaiman](https://github.com/harisvsulaiman).

## Installation

### Prerequisites

- You have [Raycast](https://www.raycast.com/) 1.26.0 or higher installed.
- You have [Node.js](https://nodejs.org/en) 16.10 or higher installed.
- You have [npm](https://www.npmjs.com/) 7.x or 8.x

## Setup

Start of by cloning this repository to your local machine into your directory of choice.

```bash
git clone https://github.com/chrisoklepke/hubspot-portal-launcher.git
```

Next run the `Import Extension` Command within Raycast and select the directory where you cloned the repository. If you can't find the command, make sure you enabled the `Developer` Commands in the Raycast preferences.

Then navigate to the folder where you cloned the repository and run the following command to create an optimized production build of the extension.

```bash
npx ray build
```

Now you should be able to use the extension and its Commands.

## Import Your Existing Portals from JSON

Instead of adding all your portals' information one by one, you're also able to import all your portals' information with the `Import Portals` Command from a JSON file.

Please note that the command doesn't validate the information you're importing. So make sure that the JSON file is formatted correctly.

The JSON file needs to be formatted like this:

```json
[
  {
    "portalId": "12345678",
    "portalName": "Acme Corp",
    "portalType": "Production"
  },
  {
    "portalId": "98765432",
    "portalName": "Acme Corp",
    "portalType": "Dev"
  },
  {
    "portalId": "78945612",
    "portalName": "Acme Corp",
    "portalType": "Test"
  }
]
```

For the `portalType` you can use the following values:

- `Production`
- `Dev`
- `Test`
- `CMS Sandbox`
- `Sandbox`

## Contribute

I'm not a developer, but learning to code with small projects like this one brings me a lot of joy. I've used a template provided by Raycast that had a lot of the functionality already, but some of the code might be a bit questionable.

However, I'm using and improving this extension for a while now, and I'm excited to share it with the community. If you have any ideas on how to improve this extension, find a bug, or like to point out some weirdness please feel free to open an issue or create a pull request.

### Why is this Extension not available in the Raycast Extension Store?

If there is enough interest in this extension, I will consider publishing it to the Raycast Store so more people, even without a developer background, can install it without the hassle.

### Shoot me a Message

If you feel like connecting or just want to talk shop, please reach out to me on [LinkedIn](https://www.linkedin.com/in/christophklepke/) or email at [chriso@conversionmate.de](mailto:chriso@conversionmate.de).
