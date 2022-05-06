# Configurable Policy Pack Example

## Prerequisites

You must have the following installed:

* [Pulumi](https://pulumi.com/docs/get-started)
* NodeJS

## Running this example

1. Clone this repo - `git clone git@github.com:pierskarsenbarg/policy-pack-stack.git`
1. Change directory - `cd polic-pack-stack`
1. Ensure you've installed the NPM packages - `npm i && cd policy && npm i && cd ..`
1. Create stack called `dev` - `pulumi stack init dev`
1. Run update targetting policy pack - `pulumi up --policy-pack ./policy` (see that you get an advisory warning. You don't have to perform the update, viewing the preview is enough)
1. Create a new stack called `prod` - `pulumi stack init prod`
1. Change the current stack to be `prod` - `pulumi stack select prod`
1. Run update (again targetting the policy pack) - `pulumi up --policy-pack ./policy` (see that you get the mandatory warning. You won't be able to perform the update)

