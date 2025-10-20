# Linux CLI

## Kaisar Provider CLI Installation Guide for Contributing to Kaisar Network

### Requirements

To run the Kaisar Provider, ensure your system meets the following specifications:

* **Operating System:** Ubuntu 20.04+, CentOS 8+, or compatible 64-bit Linux distribution
* **Memory:** 4GB RAM
* **Processor:** 64-bit CPU with virtualization support
* **Storage:** 100GB HDD/SSD
* **Internet Speed:** 100Mbps or higher

### Dependencies

The following packages and libraries are required (the setup script will install them automatically if missing):

* Node.js (v18 or higher recommended)
* npm
* pm2
* curl
* tar
* git (for some operations)

***

### 1. Download the Setup Script

Download the latest setup script from the Kaisar releases repository:

```bash
curl -O https://raw.githubusercontent.com/Kaisar-Network/kaisar-releases/main/kaisar-provider-setup.sh
```

<figure><img src="https://3420828033-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FRdDiw8sqrhonsv2Gsd47%2Fuploads%2FmRalOMd4ABB3DCtiTodx%2Fimage.png?alt=media&#x26;token=48ac7d6c-5b48-46d4-a339-b7d031115f90" alt=""><figcaption></figcaption></figure>

***

### 2. Make the Script Executable

```bash
chmod +x kaisar-provider-setup.sh
```

<figure><img src="https://3420828033-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FRdDiw8sqrhonsv2Gsd47%2Fuploads%2FWh7n6ngqPo96z0vtCpHZ%2Fimage.png?alt=media&#x26;token=56b868a3-3081-4a6b-89a9-f2d408627cf8" alt=""><figcaption></figcaption></figure>

***

### 3. Run the Setup Script with Root Privileges

```bash
sudo ./kaisar-provider-setup.sh
```

The script will automatically:

* Install Node.js, npm, and pm2 if not already present
* Download the latest release of Kaisar Provider CLI
* Install all required dependencies
* Set up the CLI globally on your system

<figure><img src="https://3420828033-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FRdDiw8sqrhonsv2Gsd47%2Fuploads%2FiyKf5BbOng6vJwoxhdrh%2Fimage.png?alt=media&#x26;token=e2ae222a-eecc-45aa-8c5a-7871ee42d66c" alt=""><figcaption></figcaption></figure>

***

### 4. Verify the Installation

After installation, verify by running:

```bash
kaisar
```

If you see a welcome message, the installation was successful!

<figure><img src="https://3420828033-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FRdDiw8sqrhonsv2Gsd47%2Fuploads%2F3JW12CaGbfzEEN5Sc93y%2Fimage.png?alt=media&#x26;token=d5cb4a62-639e-47c8-a793-7c12c2e3b0e9" alt=""><figcaption><p>kaisar command result</p></figcaption></figure>

***

### 5. Start Using the CLI

You can now join the network with the following commands:

```bash
kaisar start          # Start the Provider App
kaisar create-wallet -e <your email> # Create Wallet
kaisar import-wallet -e <your email> -k <your private key> # Import your existed wallet
kaisar status         # Check node status
kaisar log            # Check details log of Provider App
```

<figure><img src="https://3420828033-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FRdDiw8sqrhonsv2Gsd47%2Fuploads%2FAIsx8sRSdgk6lmz2BREE%2Fimage.png?alt=media&#x26;token=b519c04d-b7b3-44fd-9c2c-b500ad83f885" alt=""><figcaption></figcaption></figure>

***

**Notes:**

* Wallet and configuration data are stored in `/var/lib/kaisar-provider-cli`, so your data will not be lost when updating to a new version.
* To earn rewards, follow the instructions to create a wallet and connect your account to the Kaisar Network.

***

Good luck and enjoy earning rewards with Kaisar Network!
