# Firewall Configuration

## 1. Allow SSH Access

The following command allows SSH traffic so administrators can remotely manage the server.

```bash
sudo ufw allow ssh
```

## 2. Configure the Default Firewall Policies

The following commands deny incoming traffic by default and allow outgoing traffic.

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## 3. Enable the Firewall

The firewall was activated using the following command.

```bash
sudo ufw enable
```

To verify the firewall status and default policies, the following command was used.

```bash
sudo ufw status verbose
```

The firewall status showed that UFW was active, incoming traffic was denied by default, and outgoing traffic was allowed by default.

## 4. Allow the Web Application Port

The following command allows incoming TCP traffic on port 8080 for the Nginx web application.

```bash
sudo ufw allow 8080/tcp
```

To verify the configured firewall rules, the following command was used.

```bash
sudo ufw status numbered
```

The numbered rules can be checked to confirm that SSH and TCP port 8080 are allowed.

## 5. SSH Security Warning

If `sudo ufw enable` is executed before `sudo ufw allow ssh`, SSH connections may be blocked by the default-deny incoming policy, potentially locking administrators out of remote access to the server.
