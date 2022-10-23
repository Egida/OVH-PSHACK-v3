# OVH-PSHACK-v3

This method was used for a while to attack OVH servers (including game), it elevates CPU usage to 100%. It does not require ip spoofing since it has to perform a handshake before flooding a randomised payload and finishing the connection with a TCP FIN packet.

It can be used with servers from clouds like Oracle and DigitalOcean. Similar methods are used by skids behind stressers like stresser.us, with many free-tier machines from Oracle.

Given this method is now on the hands of certain people, I will make sure they are not the only ones to have it ;)

# Patching

It is quite easy to put an end to this method. Since there will be more than one connection being stabilished by the same ips, a ratelimit will do the job.
