Adds cs from sphinxsearch status to datadog

this adds dd-agent to the sphinxsearch group


Usage

---
- hosts:
    - all
  become: yes
  roles:
    - role: yanosliger_dev.datadog_sphinxsearch
  vars:
    metrics:
      - uptime
      - connections
      - query_wall
      - queries
      - sql_udate
