```bash
# Install/update
make

# Configure credentials
sudo blackfire-agent --register

# Start agent
sudo systemctl start blackfire-agent

# Enable auto-start after reboot
sudo systemctl enable blackfire-agent
```

## Troubleshooting

> "Probe not found, invalid signature (HTTP 200)"

Try running `sudo chmod 644 /etc/blackfire/agent` and restarting php-fpm/blackfire-agent.
