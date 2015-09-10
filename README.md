Ansible-cpufreq
===============

This is a simple ansible role for adjusting cpufrequtils preferences on Debian/Ubuntu.

Install
-------

Usage
-----

Possible parameters:
- cpufreq_enable: True|False
- cpufreq_governor: "<name of governor>"
- cpufreq_max_speed: <n>
- cpufreq_min_speed: <n>

Example usage:

    - hosts: all
      sudo: yes
      roles:
        - role: cpufreq
          cpufreq_enable: yes
          cpufreq_governor: performance
