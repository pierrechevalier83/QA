# Create Package for Vault on Windows

- [ ] Run the installer creation script `safe_vault/installer/windows/create_installer.ps1` in the safe_vault repository
- Check installer can upgrade (using default options) an existing version installed to default location which is running
  - [ ] Check test machine has older version already installed using default options and `safe_vault.exe` is running
  - [ ] Copy the current bootstrap and config files
  - [ ] New installer should run without errors
  - [ ] Check new version of `safe_vault.exe` is running and is installed in default location
  - [ ] Check bootstrap and config files haven't been overwritten
- Check installer can upgrade (using default options) an existing version installed to default location which is not running
  - [ ] Check test machine has older version already installed using default options and `safe_vault.exe` is NOT running
  - [ ] Copy the current bootstrap and config files
  - [ ] New installer should run without errors
  - [ ] Check new version of `safe_vault.exe` is running and is installed in default location
  - [ ] Check bootstrap and config files haven't been overwritten
- Check installer can upgrade (using default options) an existing version installed to non-default location which is running
  - [ ] Check test machine has older version already installed using NON-default options and `safe_vault.exe` is running
  - [ ] Copy the current bootstrap and config files
  - [ ] New installer should run without errors
  - [ ] Check new version of `safe_vault.exe` is running and is installed in default location
  - [ ] Check old version of `safe_vault.exe` has been deleted from non-default location
  - [ ] Check bootstrap and config files haven't been overwritten
- Check installer succeeds using default options on machine with no previous version installed
  - [ ] Check test machine has no version already installed
  - [ ] Installer should run without errors
  - [ ] Check new version of `safe_vault.exe` is running and is installed in default location
  - [ ] Check bootstrap and config files are installed in their default locations
- Check repair where current version installed using defaults
  - [ ] Kill and remove existing version of `safe_vault.exe`
  - [ ] Copy the current bootstrap and config files
  - [ ] Installer should run repair without errors
  - [ ] Check `safe_vault.exe` is running and has been re-installed to previous location
  - [ ] Check bootstrap and config files haven't been overwritten
  - [ ] Remove bootstrap and config files
  - [ ] Installer should run repair without errors
  - [ ] Check `safe_vault.exe` is running and is installed in previous location
- Check repair where current version installed to non-default location
  - [ ] Kill and remove existing version of `safe_vault.exe`
  - [ ] Copy the current bootstrap and config files
  - [ ] Installer should run repair without errors
  - [ ] Check `safe_vault.exe` is running and has been re-installed to previous location
  - [ ] Check bootstrap and config files haven't been overwritten
  - [ ] Remove bootstrap and config files
  - [ ] Installer should run repair without errors
  - [ ] Check `safe_vault.exe` is running and is installed in previous location
- Check uninstall where current version installed using defaults
  - [ ] Check `safe_vault.exe` is running
  - [ ] Uninstall should run without errors
  - [ ] Check `safe_vault.exe` is not running
  - [ ] Check `safe_vault.exe`, bootstrap and config files have all been removed
- Check uninstall where current version installed to non-default location
  - [ ] Check `safe_vault.exe` is running
  - [ ] Uninstall should run without errors
  - [ ] Check `safe_vault.exe` is not running
  - [ ] Check `safe_vault.exe`, bootstrap and config files have all been removed
- [ ] Copy installer from slave to website
- [ ] Update website to link to new installer
- Check installer can be downloaded
  - [ ] Webpage should detect OS and show link to appropriate installer
  - [ ] Download installer and hash check it against original
  - [ ] Check downloaded filename is meaningful
  - [ ] Check installer has appropriate high-res icon
