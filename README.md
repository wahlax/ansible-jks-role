# Java Keystore with Ansible

Role for installing and configuring a java keystore and jdk dependency.

## Optional Parameters

 * `jks_location` - Location of the Java Keystore
 * `jks_owner` - Owner of the Java Keystore
 * `jks_password` - password for the keystore
 * `jks_subject` - Details for the keystore
 * `jks_alias` - Alias for the keystore

Optional ansible-jdk-role parameters:
 * `jdk_version` - Version of JDK
 * `jdk_download_url` - URL of tar.gz for release
 * `jdk_download_sha256` - Checksum of tar.gz for release

## Testing

Credit: Tested with vagrant image from [@geerlingguy's Ansible for Devops](https://github.com/geerlingguy/ansible-for-devops)

Run the following from the test directory:

### Initial Install
```
ansible-galaxy install -r requirements.yml
vagrant up
```

### Reapply provisioning
```
vagrant provision
```
