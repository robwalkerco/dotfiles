#!/bin/bash

IP=$(dig @resolver1.opendns.com myip.opendns.com +short)

echo "My ip address is - $IP"

aws ec2 authorize-security-group-ingress --group-name ip-address-access --port 0-65535 --protocol all --cidr $IP/32