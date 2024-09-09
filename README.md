# vantage-agents-bundle
Bundle for deploying all agents required by the Vantage application

# Overview
The Vantage Agents are a custom suite of agents designed to run on HPC clusters for reporting activities to and from [Vantage](https://vantagehpc.ai). The softwares installed by the bundle are:

* [Jobbergate Agent](https://github.com/omnivector-solutions/charm-jobbergate-agent)
* [Vantage Agent](https://github.com/omnivector-solutions/charm-vantage-agent)
* [License Manager Agent](https://github.com/omnivector-solutions/charm-license-manager-agent)

# Deploy

Prior of deploying the bundle, make sure you access each agents' page and make sure you understand the configuration variables. Once you have defined the `config.yaml` file for the bundle and assuming you have *Juju* installed and ready to be used, run a single command and deploy the agents:

```python
juju deploy vantage-agents -c config.yaml
```