# Ubuntu Pro Commands

Ubuntu Pro delivers 10 years of expanded security coverage on top of Ubuntu’s Long Term Support (LTS) commitment in addition to management and compliance tooling. Visit [Ubuntu Pro](https://ubuntu.com/pro) to register for free on up to five machines.

## Activating Ubuntu Pro

- `sudo pro attach <token>`: Attaches your machine to Ubuntu Pro using a specific token. This token is provided when you subscribe to Ubuntu Pro.

## Managing Services

- `sudo pro status`: Displays the status of all Ubuntu Pro services, showing which services are enabled or disabled.
- `sudo pro enable <service>`: Enables a specific Ubuntu Pro service, such as ESM, FIPS, or Livepatch.
- `sudo pro disable <service>`: Disables a specific Ubuntu Pro service.

## Extended Security Maintenance (ESM)

- `sudo pro enable esm-infra`: Activates Extended Security Maintenance for infrastructure packages, providing security updates beyond the standard release cycle.
- `sudo pro enable esm-apps`: Activates Extended Security Maintenance for applications, extending security coverage for specific applications.

## Livepatch Service

- `sudo pro enable livepatch`: Enables the Livepatch service, which applies critical kernel patches without requiring a reboot. This helps maintain system uptime and security.

## FIPS Mode

- `sudo pro enable fips`: Enables FIPS (Federal Information Processing Standards) mode, enforcing strict cryptographic standards and practices for enhanced security compliance.

## Updating Configuration

- `sudo pro refresh`: Refreshes the Ubuntu Pro state to ensure the latest configuration and services are in place. This command updates the status and settings of Ubuntu Pro services.

## Detaching Ubuntu Pro

- `sudo pro detach`: Detaches the machine from Ubuntu Pro, disabling all services and removing the machine from the Ubuntu Pro subscription.
