# Log Analysis - Failed Login Investigation

## Context
Part of my cybersecurity learning journey (SOC - Day 1).

## Objective
Analyze authentication logs to identify suspicious login attempts.

## Commands Used
grep "Failed" auth.log
awk '{print $NF}'
sort
uniq -c

## Investigation
Filtered failed login attempts and extracted IP addresses.

## Results
The IP 192.168.1.10 made multiple failed login attempts.

## Conclusion
This behavior may indicate a brute force attack.

## Notes
Log analysis is a key skill in SOC for detecting security incidents.
