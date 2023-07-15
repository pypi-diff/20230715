# Comparing `tmp/pimelon-6.16.0.tar.gz` & `tmp/pimelon-6.16.1.tar.gz`

## Comparing `pimelon-6.16.0.tar` & `pimelon-6.16.1.tar`

### file list

```diff
@@ -1,155 +1,151 @@
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/__init__.py
--rwxr-xr-x   0        0        0    19201 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/app.py
--rwxr-xr-x   0        0        0     5720 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/cli.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/exceptions.py
--rw-r--r--   0        0        0    13252 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/pine.py
--rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/config.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/git.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/install.py
--rwxr-xr-x   0        0        0     6160 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/make.py
--rwxr-xr-x   0        0        0    12510 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/setup.py
--rwxr-xr-x   0        0        0     2805 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/update.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/commands/utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/common_site_config.py
--rwxr-xr-x   0        0        0     5393 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/lets_encrypt.py
--rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/nginx.py
--rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/procfile.py
--rwxr-xr-x   0        0        0     5531 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/production_setup.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/redis.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/site_config.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/supervisor.py
--rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/systemd.py
--rwxr-xr-x   0        0        0    38867 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/502.html
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/Procfile
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/guipine_nginx.conf
--rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/letsencrypt.cfg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/melon_sudoers
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/nginx.conf
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/nginx_default.conf
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/redis_cache.conf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/redis_queue.conf
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/redis_socketio.conf
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/supervisor.conf
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-melon-default-worker.service
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-melon-long-worker.service
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-melon-schedule.service
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-melon-short-worker.service
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-melon-web.service
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-node-socketio.service
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-redis-cache.service
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-redis-queue.service
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-redis-socketio.service
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-redis.target
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-web.target
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon-workers.target
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/config/templates/systemd/pimelon.target
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/patches/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/patches/patches.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/patches/v6/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/patches/v6/fix_backup_cronjob.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/patches/v6/fix_user_permissions.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/patches/v6/set_live_reload_config.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/patches/v6/update_archived_sites.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/create_user.yml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/macosx.yml
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/site.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/vm_build.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/bash_screen_wall/files/screen_wall.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/bash_screen_wall/tasks/main.yml
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/common/tasks/debian.yml
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/common/tasks/debian_family.yml
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/common/tasks/macos.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/common/tasks/main.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/common/tasks/redhat_family.yml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/common/tasks/ubuntu.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/dns_caching/handlers/main.yml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/dns_caching/tasks/main.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/fail2ban/defaults/main.yml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/fail2ban/handlers/main.yml
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/fail2ban/tasks/main.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/locale/defaults/main.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/locale/tasks/main.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/logwatch/defaults/main.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/logwatch/tasks/main.yml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/logwatch/templates/logwatch.conf.j2
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/README.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/defaults/main.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/files/mariadb_config.cnf
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/handlers/main.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/centos.yml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/debian.yml
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/main.yml
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/templates/my.cnf.j2
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/mariadb/vars/main.yml
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/melon_selinux/files/melon_selinux.te
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/melon_selinux/tasks/main.yml
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/README.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/defaults/main.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/handlers/main.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/meta/main.yml
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/tasks/main.yml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/tasks/setup-Debian.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/tasks/setup-RedHat.yml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/tasks/vhosts.yml
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/templates/nginx.conf.j2
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/templates/nginx.repo.j2
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/templates/vhosts.j2
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/tests/inventory
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/tests/test.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/vars/Debian.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nginx/vars/RedHat.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nodejs/defaults/main.yml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nodejs/tasks/debian_family.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nodejs/tasks/main.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/nodejs/tasks/redhat_family.yml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/ntpd/tasks/main.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/packer/tasks/debian_family.yml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/packer/tasks/main.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/packer/tasks/redhat_family.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/pine/tasks/change_ssh_port.yml
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/pine/tasks/main.yml
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/pine/tasks/setup_firewall.yml
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/pine/tasks/setup_inputrc.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/pine/tasks/setup_monak.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/pine/tasks/setup_pine_production.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/psutil/tasks/main.yml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/redis/tasks/main.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/supervisor/tasks/main.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/swap/defaults/main.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/swap/tasks/main.yml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/virtualbox/defaults/main.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/virtualbox/files/virtualbox_centos.repo
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/virtualbox/tasks/debian_family.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/virtualbox/tasks/main.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/virtualbox/tasks/redhat_family.yml
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/tests/__init__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/tests/test_base.py
--rwxr-xr-x   0        0        0     6553 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/tests/test_init.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/tests/test_setup_production.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/tests/test_utils.py
--rw-r--r--   0        0        0    13654 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/utils/__init__.py
--rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/utils/app.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/utils/cli.py
--rw-r--r--   0        0        0    18316 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/utils/pine.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/utils/render.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/utils/system.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pimelon-6.16.0/pine/utils/translation.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 pimelon-6.16.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.0/README.md
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pimelon-6.16.0/pyproject.toml
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pimelon-6.16.0/PKG-INFO
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/__init__.py
+-rwxr-xr-x   0        0        0    19232 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/app.py
+-rwxr-xr-x   0        0        0     6461 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/cli.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/exceptions.py
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/pine.py
+-rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/config.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/git.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/install.py
+-rwxr-xr-x   0        0        0     6160 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/make.py
+-rwxr-xr-x   0        0        0    12510 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/setup.py
+-rwxr-xr-x   0        0        0     2779 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/update.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/commands/utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/common_site_config.py
+-rwxr-xr-x   0        0        0     5393 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/lets_encrypt.py
+-rw-r--r--   0        0        0     8442 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/nginx.py
+-rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/procfile.py
+-rwxr-xr-x   0        0        0     5531 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/production_setup.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/redis.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/site_config.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/supervisor.py
+-rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/systemd.py
+-rwxr-xr-x   0        0        0    38867 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/502.html
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/Procfile
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/guipine_nginx.conf
+-rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/letsencrypt.cfg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/melon_sudoers
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/nginx.conf
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/nginx_default.conf
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/redis_cache.conf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/redis_queue.conf
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/redis_socketio.conf
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/supervisor.conf
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-melon-default-worker.service
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-melon-long-worker.service
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-melon-schedule.service
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-melon-short-worker.service
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-melon-web.service
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-node-socketio.service
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-redis-cache.service
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-redis-queue.service
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-redis-socketio.service
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-redis.target
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-web.target
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon-workers.target
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/config/templates/systemd/pimelon.target
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/patches/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/patches/patches.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/patches/v6/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/patches/v6/fix_backup_cronjob.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/patches/v6/fix_user_permissions.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/patches/v6/set_live_reload_config.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/patches/v6/update_archived_sites.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/create_user.yml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/macosx.yml
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/site.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/vm_build.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/bash_screen_wall/files/screen_wall.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/bash_screen_wall/tasks/main.yml
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/common/tasks/debian.yml
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/common/tasks/debian_family.yml
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/common/tasks/macos.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/common/tasks/main.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/common/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/common/tasks/ubuntu.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/dns_caching/handlers/main.yml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/dns_caching/tasks/main.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/fail2ban/defaults/main.yml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/fail2ban/handlers/main.yml
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/fail2ban/tasks/main.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/locale/defaults/main.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/locale/tasks/main.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/logwatch/defaults/main.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/logwatch/tasks/main.yml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/logwatch/templates/logwatch.conf.j2
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/README.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/defaults/main.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/files/mariadb_config.cnf
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/handlers/main.yml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/centos.yml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/debian.yml
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/main.yml
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/templates/my.cnf.j2
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/mariadb/vars/main.yml
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/melon_selinux/files/melon_selinux.te
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/melon_selinux/tasks/main.yml
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/README.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/defaults/main.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/handlers/main.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/meta/main.yml
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/tasks/main.yml
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/tasks/setup-Debian.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/tasks/setup-RedHat.yml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/tasks/vhosts.yml
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/templates/nginx.conf.j2
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/templates/nginx.repo.j2
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/templates/vhosts.j2
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/tests/inventory
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/tests/test.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/vars/Debian.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nginx/vars/RedHat.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nodejs/defaults/main.yml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nodejs/tasks/debian_family.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nodejs/tasks/main.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/nodejs/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/ntpd/tasks/main.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/packer/tasks/debian_family.yml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/packer/tasks/main.yml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/packer/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/pine/tasks/change_ssh_port.yml
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/pine/tasks/main.yml
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/pine/tasks/setup_firewall.yml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/pine/tasks/setup_inputrc.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/pine/tasks/setup_monak.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/pine/tasks/setup_pine_production.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/psutil/tasks/main.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/redis/tasks/main.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/supervisor/tasks/main.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/swap/defaults/main.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/swap/tasks/main.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/virtualbox/defaults/main.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/virtualbox/files/virtualbox_centos.repo
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/virtualbox/tasks/debian_family.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/virtualbox/tasks/main.yml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/virtualbox/tasks/redhat_family.yml
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/tests/__init__.py
+-rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/utils/__init__.py
+-rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/utils/app.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/utils/cli.py
+-rw-r--r--   0        0        0    18108 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/utils/pine.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/utils/render.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/utils/system.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pimelon-6.16.1/pine/utils/translation.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 pimelon-6.16.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pimelon-6.16.1/README.md
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pimelon-6.16.1/pyproject.toml
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pimelon-6.16.1/PKG-INFO
```

### Comparing `pimelon-6.16.0/pine/app.py` & `pimelon-6.16.1/pine/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,26 +179,26 @@
 		self.pine.run(
 			f"{cmd} {args}",
 			cwd=os.path.join(self.pine.name, "apps"),
 		)
 
 	@step(title="Archiving App {repo}", success="App {repo} Archived")
 	def remove(self, no_backup: bool = False):
-		active_app_path = os.path.join("apps", self.repo)
+		active_app_path = os.path.join("apps", self.app_name)
 
 		if no_backup:
 			if not os.path.islink(active_app_path):
 				shutil.rmtree(active_app_path)
 			else:
 				os.remove(active_app_path)
 			log(f"App deleted from {active_app_path}")
 		else:
 			archived_path = os.path.join("archived", "apps")
 			archived_name = get_available_folder_name(
-				f"{self.repo}-{date.today()}", archived_path
+				f"{self.app_name}-{date.today()}", archived_path
 			)
 			archived_app_path = os.path.join(archived_path, archived_name)
 
 			shutil.move(active_app_path, archived_app_path)
 			log(f"App moved from {active_app_path} to {archived_app_path}")
 
 		self.from_apps = False
@@ -214,15 +214,15 @@
 		ignore_resolution=False,
 	):
 		import pine.cli
 		from pine.utils.app import get_app_name
 
 		verbose = pine.cli.verbose or verbose
 		app_name = get_app_name(self.pine.name, self.app_name)
-		if not resolved and self.repo != "melon" and not ignore_resolution:
+		if not resolved and self.app_name != "melon" and not ignore_resolution:
 			click.secho(
 				f"Ignoring dependencies of {self.name}. To install dependencies use --resolve-deps",
 				fg="yellow",
 			)
 
 		install_app(
 			app=app_name,
@@ -243,15 +243,15 @@
 	def uninstall(self):
 		self.pine.run(f"{self.pine.python} -m pip uninstall -y {self.name}")
 
 	def _get_dependencies(self):
 		from pine.utils.app import get_required_deps, required_apps_from_hooks
 
 		if self.on_disk:
-			required_deps = os.path.join(self.mount_path, self.repo, "hooks.py")
+			required_deps = os.path.join(self.mount_path, self.app_name, "hooks.py")
 			try:
 				return required_apps_from_hooks(required_deps, local=True)
 			except IndexError:
 				return []
 		try:
 			required_deps = get_required_deps(self.org, self.repo, self.tag or self.branch)
 			return required_apps_from_hooks(required_deps)
@@ -271,24 +271,24 @@
 
 
 def make_resolution_plan(app: App, pine: "Pine"):
 	"""
 	decide what apps and versions to install and in what order
 	"""
 	resolution = OrderedDict()
-	resolution[app.repo] = app
+	resolution[app.app_name] = app
 
 	for app_name in app._get_dependencies():
 		dep_app = App(app_name, pine=pine)
 		is_valid_melon_branch(dep_app.url, dep_app.branch)
 		dep_app.required_by = app.name
-		if dep_app.repo in resolution:
-			click.secho(f"{dep_app.repo} is already resolved skipping", fg="yellow")
+		if dep_app.app_name in resolution:
+			click.secho(f"{dep_app.app_name} is already resolved skipping", fg="yellow")
 			continue
-		resolution[dep_app.repo] = dep_app
+		resolution[dep_app.app_name] = dep_app
 		resolution.update(make_resolution_plan(dep_app, pine))
 		app.local_resolution = [repo_name for repo_name, _ in reversed(resolution.items())]
 	return resolution
 
 
 def get_excluded_apps(pine_path="."):
 	try:
@@ -296,15 +296,15 @@
 			return f.read().strip().split("\n")
 	except OSError:
 		return []
 
 
 def add_to_excluded_apps_txt(app, pine_path="."):
 	if app == "melon":
-		raise ValueError("Melon app cannot be excludeed from update")
+		raise ValueError("Melon app cannot be excluded from update")
 	if app not in os.listdir("apps"):
 		raise ValueError(f"The app {app} does not exist")
 	apps = get_excluded_apps(pine_path=pine_path)
 	if app not in apps:
 		apps.append(app)
 		return write_excluded_apps_txt(apps, pine_path=pine_path)
 
@@ -602,16 +602,16 @@
 
 Cannot proceed with update: You have local changes in app "{app}" that are not committed.
 
 Here are your choices:
 
 1. Merge the {app} app manually with "git pull" / "git pull --rebase" and fix conflicts.
 1. Temporarily remove your changes with "git stash" or discard them completely
-	with "pine update --reset" or for individual repositries "git reset --hard".
-"""
+	with "pine update --reset" or for individual repositries "git reset --hard"
+	"""
 					)
 					sys.exit(1)
 
 	for app in apps:
 		if app in excluded_apps:
 			print(f"Skipping pull for app {app}")
 			continue
```

### Comparing `pimelon-6.16.0/pine/cli.py` & `pimelon-6.16.1/pine/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,24 +24,27 @@
 	is_dist_editable,
 	is_root,
 	log,
 	setup_logging,
 	get_cmd_from_sysargv,
 )
 from pine.utils.pine import get_env_cmd
+from importlib.util import find_spec
+
 
 # these variables are used to show dynamic outputs on the terminal
 dynamic_feed = False
 verbose = False
 is_envvar_warn_set = None
 from_command_line = False  # set when commands are executed via the CLI
 pine.LOG_BUFFER = []
 
 change_uid_msg = "You should not run this command as root"
 src = os.path.dirname(__file__)
+SKIP_MODULE_TRACEBACK = ("click",)
 
 
 @contextmanager
 def execute_cmd(check_for_update=True, command: str = None, logger: Logger = None):
 	if check_for_update:
 		atexit.register(check_latest_version)
 
@@ -114,14 +117,16 @@
 		if in_pine:
 			print(get_melon_help())
 		return
 
 	_opts = [x.opts + x.secondary_opts for x in pine_command.params]
 	opts = {item for sublist in _opts for item in sublist}
 
+	setup_exception_handler()
+
 	# handle usages like `--use-feature='feat-x'` and `--use-feature 'feat-x'`
 	if cmd_from_sys and cmd_from_sys.split("=", 1)[0].strip() in opts:
 		pine_command()
 
 	if cmd_from_sys in pine_command.commands:
 		with execute_cmd(check_for_update=is_cli_command, command=command, logger=logger):
 			pine_command()
@@ -236,7 +241,30 @@
 
 	def _chdir(*args, **kwargs):
 		Pine.cache_clear()
 		get_env_cmd.cache_clear()
 		return f(*args, **kwargs)
 
 	os.chdir = _chdir
+
+
+def setup_exception_handler():
+	from traceback import format_exception
+	from pine.exceptions import CommandFailedError
+
+	def handle_exception(exc_type, exc_info, tb):
+		if exc_type == CommandFailedError:
+			print("".join(generate_exc(exc_type, exc_info, tb)))
+		else:
+			sys.__excepthook__(exc_type, exc_info, tb)
+
+	def generate_exc(exc_type, exc_info, tb):
+		TB_SKIP = [
+			os.path.dirname(find_spec(module).origin) for module in SKIP_MODULE_TRACEBACK
+		]
+
+		for tb_line in format_exception(exc_type, exc_info, tb):
+			for skip_module in TB_SKIP:
+				if skip_module not in tb_line:
+					yield tb_line
+
+	sys.excepthook = handle_exception
```

### Comparing `pimelon-6.16.0/pine/exceptions.py` & `pimelon-6.16.1/pine/exceptions.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/pine.py` & `pimelon-6.16.1/pine/pine.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 		if not force:
 			self.validate_app_uninstall(app)
 		try:
 			self.apps.remove(App(app, pine=self, to_clone=False), no_backup=no_backup)
 		except InvalidRemoteException:
 			if not force:
 				raise
+
 		self.apps.sync()
 		# self.build() - removed because it seems unnecessary
 		self.reload(_raise=False)
 
 	@step(title="Building Pine Assets", success="Pine Assets Built")
 	def build(self):
 		# build assets & stuff
@@ -305,21 +306,21 @@
 		"""add an item, value, at index, key."""
 		# TODO: fetch and install app to pine
 		self.apps.insert(key, value)
 
 	def add(self, app: "App"):
 		app.get()
 		app.install()
-		super().append(app.repo)
+		super().append(app.app_name)
 		self.apps.sort()
 
 	def remove(self, app: "App", no_backup: bool = False):
 		app.uninstall()
 		app.remove(no_backup=no_backup)
-		super().remove(app.repo)
+		super().remove(app.app_name)
 
 	def append(self, app: "App"):
 		return self.add(app)
 
 	def __repr__(self):
 		return self.__str__()
 
@@ -436,17 +437,17 @@
 		logfile = os.path.join(pine_dir, "logs", "backup.log")
 		system_crontab = CronTab(user=user)
 		backup_command = f"cd {pine_dir} && {sys.argv[0]} --verbose --site all backup"
 		job_command = f"{backup_command} >> {logfile} 2>&1"
 
 		if job_command not in str(system_crontab):
 			job = system_crontab.new(
-				command=job_command, comment="pine auto backups set for every 12 hours"
+				command=job_command, comment="pine auto backups set for every 8 hours"
 			)
-			job.every(12).hours()
+			job.every(8).hours()
 			system_crontab.write()
 
 		logger.log("backups were set up")
 
 	@job(title="Setting Up Pine Dependencies", success="Pine Dependencies Set Up")
 	def requirements(self, apps=None):
 		"""Install and upgrade specified / all installed apps on given Pine"""
```

### Comparing `pimelon-6.16.0/pine/commands/__init__.py` & `pimelon-6.16.1/pine/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/commands/config.py` & `pimelon-6.16.1/pine/commands/config.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/commands/git.py` & `pimelon-6.16.1/pine/commands/git.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/commands/install.py` & `pimelon-6.16.1/pine/commands/install.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/commands/make.py` & `pimelon-6.16.1/pine/commands/make.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/commands/setup.py` & `pimelon-6.16.1/pine/commands/setup.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/commands/update.py` & `pimelon-6.16.1/pine/commands/update.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	"--no-backup",
 	is_flag=True,
 	help="If this flag is set, sites won't be backed up prior to updates. Note: This is not recommended in production.",
 )
 @click.option(
 	"--no-compile",
 	is_flag=True,
-	help="If set, Python bytecode won't be compiled before restarting the processes",
+	help="[DEPRECATED] This flag doesn't do anything now.",
 )
 @click.option("--force", is_flag=True, help="Forces major version upgrades")
 @click.option(
 	"--reset",
 	is_flag=True,
 	help="Hard resets git branch's to their new states overriding any changes and overriding rebase on pull",
 )
```

### Comparing `pimelon-6.16.0/pine/commands/utils.py` & `pimelon-6.16.1/pine/commands/utils.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/common_site_config.py` & `pimelon-6.16.1/pine/config/common_site_config.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/lets_encrypt.py` & `pimelon-6.16.1/pine/config/lets_encrypt.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/nginx.py` & `pimelon-6.16.1/pine/config/nginx.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/procfile.py` & `pimelon-6.16.1/pine/config/procfile.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/production_setup.py` & `pimelon-6.16.1/pine/config/production_setup.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/redis.py` & `pimelon-6.16.1/pine/config/redis.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/site_config.py` & `pimelon-6.16.1/pine/config/site_config.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/supervisor.py` & `pimelon-6.16.1/pine/config/supervisor.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
 	for possibility in possibilities:
 		if os.path.exists(possibility):
 			return possibility
 
 
 def check_supervisord_config(user=None):
-	"""From pine v5.x, we're moving to supervisor running as user"""
 	import configparser
 
 	if not user:
 		user = getpass.getuser()
 
 	supervisord_conf = get_supervisord_conf()
 	section = "unix_http_server"
```

### Comparing `pimelon-6.16.0/pine/config/systemd.py` & `pimelon-6.16.1/pine/config/systemd.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/templates/502.html` & `pimelon-6.16.1/pine/config/templates/502.html`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/templates/Procfile` & `pimelon-6.16.1/pine/config/templates/Procfile`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/templates/guipine_nginx.conf` & `pimelon-6.16.1/pine/config/templates/guipine_nginx.conf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/templates/letsencrypt.cfg` & `pimelon-6.16.1/pine/config/templates/letsencrypt.cfg`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/templates/nginx.conf` & `pimelon-6.16.1/pine/config/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/templates/nginx_default.conf` & `pimelon-6.16.1/pine/config/templates/nginx_default.conf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/config/templates/supervisor.conf` & `pimelon-6.16.1/pine/config/templates/supervisor.conf`

 * *Files 2% similar despite different names*

```diff
@@ -178,20 +178,20 @@
 
 [group:{{ pine_name }}-web]
 programs={{ pine_name }}-melon-web {%- if node -%} ,{{ pine_name }}-node-socketio {%- endif%}
 
 {% if use_rq %}
 
 [group:{{ pine_name }}-workers]
-programs={{ pine_name }}-melon-schedule,{{ pine_name }}-melon-default-worker,{{ pine_name }}-melon-short-worker,{{ pine_name }}-melon-long-worker
+programs={{ pine_name }}-melon-schedule,{{ pine_name }}-melon-default-worker,{{ pine_name }}-melon-short-worker,{{ pine_name }}-melon-long-worker{%- for worker_name in workers -%},{{ pine_name }}-melon-{{ worker_name }}-worker{%- endfor %}
 
 {% else %}
 
 [group:{{ pine_name }}-workers]
-programs={{ pine_name }}-melon-workerbeat,{{ pine_name }}-melon-worker,{{ pine_name }}-melon-longjob-worker,{{ pine_name }}-melon-async-worker
+programs={{ pine_name }}-melon-workerbeat,{{ pine_name }}-melon-worker,{{ pine_name }}-melon-longjob-worker,{{ pine_name }}-melon-async-worker{%- for worker_name in workers -%},{{ pine_name }}-melon-{{ worker_name }}-worker{%- endfor %}
 
 {% endif %}
 
 {% if not skip_redis %}
 [group:{{ pine_name }}-redis]
 programs={{ pine_name }}-redis-cache,{{ pine_name }}-redis-queue,{{ pine_name }}-redis-socketio
 {% endif %}
```

### Comparing `pimelon-6.16.0/pine/config/templates/systemd/pimelon-melon-web.service` & `pimelon-6.16.1/pine/config/templates/systemd/pimelon-melon-web.service`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/patches/__init__.py` & `pimelon-6.16.1/pine/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/patches/v6/fix_user_permissions.py` & `pimelon-6.16.1/pine/patches/v6/fix_user_permissions.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/patches/v6/update_archived_sites.py` & `pimelon-6.16.1/pine/patches/v6/update_archived_sites.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/create_user.yml` & `pimelon-6.16.1/pine/playbooks/create_user.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/macosx.yml` & `pimelon-6.16.1/pine/playbooks/macosx.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/site.yml` & `pimelon-6.16.1/pine/playbooks/site.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/common/tasks/debian.yml` & `pimelon-6.16.1/pine/playbooks/roles/common/tasks/debian.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/common/tasks/debian_family.yml` & `pimelon-6.16.1/pine/playbooks/roles/common/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/common/tasks/macos.yml` & `pimelon-6.16.1/pine/playbooks/roles/common/tasks/macos.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/common/tasks/redhat_family.yml` & `pimelon-6.16.1/pine/playbooks/roles/common/tasks/redhat_family.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/common/tasks/ubuntu.yml` & `pimelon-6.16.1/pine/playbooks/roles/common/tasks/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/fail2ban/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/fail2ban/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2` & `pimelon-6.16.1/pine/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/locale/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/locale/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/mariadb/README.md` & `pimelon-6.16.1/pine/playbooks/roles/mariadb/README.md`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/mariadb/files/mariadb_config.cnf` & `pimelon-6.16.1/pine/playbooks/roles/mariadb/files/mariadb_config.cnf`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/debian.yml` & `pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/debian.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml` & `pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml` & `pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml` & `pimelon-6.16.1/pine/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/melon_selinux/files/melon_selinux.te` & `pimelon-6.16.1/pine/playbooks/roles/melon_selinux/files/melon_selinux.te`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/melon_selinux/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/melon_selinux/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/nginx/README.md` & `pimelon-6.16.1/pine/playbooks/roles/nginx/README.md`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/nginx/defaults/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/nginx/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/nginx/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/nginx/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/nginx/tasks/setup-Debian.yml` & `pimelon-6.16.1/pine/playbooks/roles/nginx/tasks/setup-Debian.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/nginx/tasks/vhosts.yml` & `pimelon-6.16.1/pine/playbooks/roles/nginx/tasks/vhosts.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/nginx/templates/nginx.conf.j2` & `pimelon-6.16.1/pine/playbooks/roles/nginx/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/nginx/templates/vhosts.j2` & `pimelon-6.16.1/pine/playbooks/roles/nginx/templates/vhosts.j2`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/ntpd/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/ntpd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/packer/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/packer/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/pine/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/pine/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/pine/tasks/setup_firewall.yml` & `pimelon-6.16.1/pine/playbooks/roles/pine/tasks/setup_firewall.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/pine/tasks/setup_monak.yml` & `pimelon-6.16.1/pine/playbooks/roles/pine/tasks/setup_monak.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/pine/tasks/setup_pine_production.yml` & `pimelon-6.16.1/pine/playbooks/roles/pine/tasks/setup_pine_production.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/redis/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/redis/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/swap/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/swap/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/virtualbox/tasks/debian_family.yml` & `pimelon-6.16.1/pine/playbooks/roles/virtualbox/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml` & `pimelon-6.16.1/pine/playbooks/roles/wkhtmltopdf/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/utils/__init__.py` & `pimelon-6.16.1/pine/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 	cmd_log = f"{cwd_info}{cmd}"
 	logger.debug(cmd_log)
 	spl_cmd = split(cmd)
 	return_code = subprocess.call(spl_cmd, cwd=cwd, universal_newlines=True, env=env)
 	if return_code:
 		logger.warning(f"{cmd_log} executed with exit code {return_code}")
 		if _raise:
-			raise CommandFailedError from subprocess.CalledProcessError(return_code, cmd)
+			raise CommandFailedError(cmd) from subprocess.CalledProcessError(return_code, cmd)
 	return return_code
 
 
 def which(executable: str, raise_err: bool = False) -> str:
 	from shutil import which
 
 	exec_ = which(executable)
@@ -522,16 +522,16 @@
 	def copy(self):
 		return _dict(dict(self).copy())
 
 
 def get_cmd_from_sysargv():
 	"""Identify and segregate tokens to options and command
 
-	For Command: `pine --profile --site melon.monakerp.com migrate --no-backup`
-	sys.argv: ["/home/melon/.local/bin/pine", "--profile", "--site", "melon.monakerp.com", "migrate", "--no-backup"]
+	For Command: `pine --profile --site monakerp.com migrate --no-backup`
+	sys.argv: ["/home/melon/.local/bin/pine", "--profile", "--site", "monakerp.com", "migrate", "--no-backup"]
 	Actual command run: migrate
 
 	"""
 	# context is passed as options to melon's pine_helper
 	from pine.pine import Pine
 
 	melon_context = _dict(params={"--site"}, flags={"--verbose", "--profile", "--force"})
```

### Comparing `pimelon-6.16.0/pine/utils/app.py` & `pimelon-6.16.1/pine/utils/app.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/utils/cli.py` & `pimelon-6.16.1/pine/utils/cli.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/utils/pine.py` & `pimelon-6.16.1/pine/utils/pine.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,15 @@
 	print("Updating node packages...")
 	from distutils.version import LooseVersion
 
 	from pine.utils.app import get_develop_version
 
 	v = LooseVersion(get_develop_version("melon", pine_path=pine_path))
 
-	# if develop_verion is 4 and up, only then install yarn
-	if v < LooseVersion("4.x.x-develop"):
-		update_npm_packages(pine_path, apps=apps)
-	else:
-		update_yarn_packages(pine_path, apps=apps)
+	update_yarn_packages(pine_path, apps=apps)
 
 
 def install_python_dev_dependencies(pine_path=".", apps=None, verbose=False):
 	import pine.cli
 	from pine.pine import Pine
 
 	verbose = pine.cli.verbose or verbose
@@ -150,15 +146,15 @@
 						if isinstance(value, dict):
 							package_json[key].update(value)
 						elif isinstance(value, list):
 							package_json[key].extend(value)
 						else:
 							package_json[key] = value
 
-	if package_json is {}:
+	if package_json == {}:
 		with open(os.path.join(os.path.dirname(__file__), "package.json")) as f:
 			package_json = json.loads(f.read())
 
 	with open(os.path.join(pine_path, "package.json"), "w") as f:
 		f.write(json.dumps(package_json, indent=1, sort_keys=True))
 
 	exec_cmd("npm install", cwd=pine_path)
@@ -451,28 +447,21 @@
 	if build:
 		print("Building assets...")
 		pine.build()
 
 	if version_upgrade[0] or (not version_upgrade[0] and force):
 		post_upgrade(version_upgrade[1], version_upgrade[2], pine_path=pine_path)
 
-	if pull and compile:
-		from compileall import compile_dir
-
-		print("Compiling Python files...")
-		apps_dir = os.path.join(pine_path, "apps")
-		compile_dir(apps_dir, quiet=1, rx=re.compile(".*node_modules.*"))
-
 	pine.reload(web=False, supervisor=restart_supervisor, systemd=restart_systemd)
 
 	conf.update({"maintenance_mode": 0, "pause_scheduler": 0})
 	update_config(conf, pine_path=pine_path)
 
 	print(
-		"_" * 80 + "\nPine: Deployment tool for MonakERP and MonakERP Applications"
+		"_" * 80 + "\nPine: Deployment tool for MonakERP Applications"
 	)
 
 
 def clone_apps_from(pine_path, clone_from, update_app=True):
 	from pine.app import install_app
 
 	print(f"Copying apps from {clone_from}...")
@@ -616,12 +605,19 @@
 
 	for app in intersection_apps:
 		branch = get_current_branch(app)
 
 		if branch == "master":
 			print(
 				"""'master' branch is renamed to 'version-4' since 'version-5' release.
+As of January 2020, the following branches are
+version		Melon			Monak
+4		version-4		version-4
+5		version-5		version-5
+6		version-6		version-6
+7		develop			develop
+
 Please switch to new branches to get future updates.
 To switch to your required branch, run the following commands: pine switch-to-branch [branch-name]"""
 			)
 
 			sys.exit(1)
```

### Comparing `pimelon-6.16.0/pine/utils/render.py` & `pimelon-6.16.1/pine/utils/render.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/utils/system.py` & `pimelon-6.16.1/pine/utils/system.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pine/utils/translation.py` & `pimelon-6.16.1/pine/utils/translation.py`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/.gitignore` & `pimelon-6.16.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pimelon-6.16.0/pyproject.toml` & `pimelon-6.16.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: System :: Installation/Setup",
 ]
 dependencies = [
     "Click>=7.0",
-    "GitPython~=2.1.15",
+    "GitPython~=3.1.30",
     "honcho",
     "Jinja2~=3.0.3",
     "python-crontab~=2.6.0",
     "requests",
     "semantic-version~=2.8.2",
     "setuptools>40.9.0",
     "tomli;python_version<'3.11'",
```

### Comparing `pimelon-6.16.0/PKG-INFO` & `pimelon-6.16.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pimelon
-Version: 6.16.0
+Version: 6.16.1
 Summary: CLI to manage Multi-tenant deployments for Monakerp apps
 Project-URL: Homepage, https://monakerp.com/pine
 Project-URL: Source, https://github.com/amonak/pine
 Author-email: Alphamonak Solutions <amonak@monakerp.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -12,15 +12,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: System :: Installation/Setup
 Requires-Python: >=3.7
 Requires-Dist: click>=7.0
-Requires-Dist: gitpython~=2.1.15
+Requires-Dist: gitpython~=3.1.30
 Requires-Dist: honcho
 Requires-Dist: jinja2~=3.0.3
 Requires-Dist: python-crontab~=2.6.0
 Requires-Dist: requests
 Requires-Dist: semantic-version~=2.8.2
 Requires-Dist: setuptools>40.9.0
 Requires-Dist: tomli; python_version < '3.11'
```

