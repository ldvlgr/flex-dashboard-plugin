# Your custom Twilio Flex Plugin

Twilio Flex Plugins allow you to customize the appearance and behavior of [Twilio Flex](https://www.twilio.com/flex). If you want to learn more about the capabilities and how to use the API, check out our [Flex documentation](https://www.twilio.com/docs/flex).


This plugin was created with 
```
twilio flex:plugins:create flex-dashboard-plugin --install --flexui2 --typescript
```

## Feature Summary
This plugin includes a customization to allow Flex [Supervisor Users]((https://www.twilio.com/docs/flex/onboarding-guide/set-up-your-flex-account#flex-user-roles)) with reduced (view only) permissions to see the Teams View but not make any changes to the agent activity or update their skills.

For any user with the Supervisor role and the worker attribute `agent_lead = true`, we will remove the Profile component (Activity select) and [Skills components](https://www.twilio.com/docs/flex/onboarding-guide/configure-skill-based-routing#assign-a-skill-to-an-agent) from the [Worker Canvas](https://assets.flex.twilio.com/docs/releases/flex-ui/2.4.1/programmable-components/components/WorkerCanvas/).



## Setup

See the [Plugins Quickstart guide](https://www.twilio.com/docs/flex/quickstart/getting-started-plugin) for more information.



Make sure you have [Node.js](https://nodejs.org) as well as [`npm`](https://npmjs.com). We support Node >= 10.12 (and recommend the _even_ versions of Node). Afterwards, install the dependencies by running `npm install`:

```bash
cd 

# If you use npm
npm install
```

Next, please install the [Twilio CLI](https://www.twilio.com/docs/twilio-cli/quickstart) by running:

```bash
brew tap twilio/brew && brew install twilio
```

Finally, install the [Flex Plugin extension](https://github.com/twilio-labs/plugin-flex/tree/v1-beta) for the Twilio CLI:

```bash
twilio plugins:install @twilio-labs/plugin-flex
```

## Development

Run `twilio flex:plugins --help` to see all the commands we currently support. For further details on Flex Plugins refer to our documentation on the [Twilio Docs](https://www.twilio.com/docs/flex/developer/plugins/cli) page.

