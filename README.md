# cloudformation-guard ECS task definition example

with VSCode remote containers configurations.

See also [this repo](https://github.com/aws-cloudformation/cloudformation-guard) for futher information about cloudformation-guard.

## Setup

1. Clone this repo
2. Spin up a devcontainer within Visual Studio Code (This may take several minutes to build Rust and the cfn-guard/cfn-guard-rulegen binaries, have a coffee break ☕️)

## Usage

1. After the setup, open a new terminal in the VSCode window
2. Try `cfn-guard -t examples/cfn-yamls/compliant.yaml -r examples/rules/ecs_taskdef_template.ruleset` to test a compliant CFn template
3. Try `cfn-guard -t examples/cfn-yamls/uncompliant.yaml -r examples/rules/ecs_taskdef_template.ruleset` to test an uncompliant CFn template, and you'll see some validation errors :)

## Author

[Tori](https://github.com/toricls)
