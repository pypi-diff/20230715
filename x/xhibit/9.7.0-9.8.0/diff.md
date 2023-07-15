# Comparing `tmp/xhibit-9.7.0.tar.gz` & `tmp/xhibit-9.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhibit-9.7.0.tar", last modified: Fri Jul 14 08:24:26 2023, max compression
+gzip compressed data, was "xhibit-9.8.0.tar", last modified: Sat Jul 15 18:29:38 2023, max compression
```

## Comparing `xhibit-9.7.0.tar` & `xhibit-9.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 08:24:26.839144 xhibit-9.7.0/
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 08:24:26.838144 xhibit-9.7.0/Exhibition/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 08:15:10.000000 xhibit-9.7.0/Exhibition/__init__.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 08:15:10.000000 xhibit-9.7.0/Exhibition/ascii.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 08:15:10.000000 xhibit-9.7.0/Exhibition/color_palette.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 08:15:10.000000 xhibit-9.7.0/Exhibition/colors.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2736 2023-07-14 08:15:10.000000 xhibit-9.7.0/Exhibition/image.py
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 08:15:10.000000 xhibit-9.7.0/Exhibition/pos.sh
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)    16167 2023-07-14 08:24:17.000000 xhibit-9.7.0/Exhibition/shell.sh
--rw-r--r--   0 ayush     (1000) ayush     (1000)      730 2023-07-14 08:15:10.000000 xhibit-9.7.0/Exhibition/sysinfo.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 08:15:10.000000 xhibit-9.7.0/LICENSE
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4339 2023-07-14 08:24:26.839144 xhibit-9.7.0/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3785 2023-07-14 08:15:10.000000 xhibit-9.7.0/README.md
--rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 08:24:26.839144 xhibit-9.7.0/setup.cfg
--rw-r--r--   0 ayush     (1000) ayush     (1000)      975 2023-07-14 08:24:24.000000 xhibit-9.7.0/setup.py
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 08:24:26.839144 xhibit-9.7.0/xhibit.egg-info/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4339 2023-07-14 08:24:26.000000 xhibit-9.7.0/xhibit.egg-info/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 08:24:26.000000 xhibit-9.7.0/xhibit.egg-info/SOURCES.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 08:24:26.000000 xhibit-9.7.0/xhibit.egg-info/dependency_links.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 08:24:26.000000 xhibit-9.7.0/xhibit.egg-info/entry_points.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 08:24:26.000000 xhibit-9.7.0/xhibit.egg-info/requires.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 08:24:26.000000 xhibit-9.7.0/xhibit.egg-info/top_level.txt
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-15 18:29:38.612148 xhibit-9.8.0/
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-15 18:29:38.612148 xhibit-9.8.0/Exhibition/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-15 16:45:18.000000 xhibit-9.8.0/Exhibition/__init__.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-15 16:45:18.000000 xhibit-9.8.0/Exhibition/ascii.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-15 16:45:18.000000 xhibit-9.8.0/Exhibition/color_palette.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-15 16:45:18.000000 xhibit-9.8.0/Exhibition/colors.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2736 2023-07-15 16:45:18.000000 xhibit-9.8.0/Exhibition/image.py
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-15 16:45:18.000000 xhibit-9.8.0/Exhibition/pos.sh
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)    22347 2023-07-15 18:28:32.000000 xhibit-9.8.0/Exhibition/shell.sh
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      730 2023-07-15 16:45:18.000000 xhibit-9.8.0/Exhibition/sysinfo.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-15 16:45:18.000000 xhibit-9.8.0/LICENSE
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4339 2023-07-15 18:29:38.612148 xhibit-9.8.0/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3785 2023-07-15 16:45:18.000000 xhibit-9.8.0/README.md
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-15 18:29:38.613149 xhibit-9.8.0/setup.cfg
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      975 2023-07-15 18:28:47.000000 xhibit-9.8.0/setup.py
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-15 18:29:38.612148 xhibit-9.8.0/xhibit.egg-info/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4339 2023-07-15 18:29:38.000000 xhibit-9.8.0/xhibit.egg-info/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-15 18:29:38.000000 xhibit-9.8.0/xhibit.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-15 18:29:38.000000 xhibit-9.8.0/xhibit.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-15 18:29:38.000000 xhibit-9.8.0/xhibit.egg-info/entry_points.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-15 18:29:38.000000 xhibit-9.8.0/xhibit.egg-info/requires.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-15 18:29:38.000000 xhibit-9.8.0/xhibit.egg-info/top_level.txt
```

### Comparing `xhibit-9.7.0/Exhibition/__init__.py` & `xhibit-9.8.0/Exhibition/__init__.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/Exhibition/ascii.py` & `xhibit-9.8.0/Exhibition/ascii.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/Exhibition/color_palette.py` & `xhibit-9.8.0/Exhibition/color_palette.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/Exhibition/colors.py` & `xhibit-9.8.0/Exhibition/colors.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/Exhibition/image.py` & `xhibit-9.8.0/Exhibition/image.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/Exhibition/pos.sh` & `xhibit-9.8.0/Exhibition/pos.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/Exhibition/shell.sh` & `xhibit-9.8.0/Exhibition/shell.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,67 @@
 #!/usr/bin/env bash
 
+# Utility Function
+get_kernel() {
+    # Since these OS are integrated systems, it's better to skip this function altogether
+    [[ $os =~ (AIX|IRIX) ]] && return
+
+    # Haiku uses 'uname -v' and not - 'uname -r'.
+    [[ $os == Haiku ]] && {
+        kernel=$(uname -v)
+        return
+    }
+
+    # In Windows 'uname' may return the info of GNUenv thus use wmic for OS kernel.
+    [[ $os == Windows ]] && {
+        kernel=$(wmic os get Version)
+        kernel=${kernel/Version}
+        return
+    }
+
+    case $kernel_shorthand in
+        on)  kernel=$kernel_version ;;
+        off) kernel="$kernel_name $kernel_version" ;;
+    esac
+
+    # Hide kernel info if it's identical to the distro info.
+    [[ $os =~ (BSD|MINIX) && $distro == *"$kernel_name"* ]] &&
+    case $distro_shorthand in
+        on|tiny) kernel=$kernel_version ;;
+        *)       unset kernel ;;
+    esac
+}
+
+# Utility Function
+cache_uname() {
+    # Cache the output of uname so we don't
+    # have to spawn it multiple times.
+    IFS=" " read -ra uname <<< "$(uname -srm)"
+
+    kernel_name="${uname[0]}"
+    kernel_version="${uname[1]}"
+    kernel_machine="${uname[2]}"
+
+    if [[ "$kernel_name" == "Darwin" ]]; then
+        # macOS can report incorrect versions unless this is 0.
+        # https://github.com/dylanaraps/neofetch/issues/1607
+        export SYSTEM_VERSION_COMPAT=0
+
+        IFS=$'\n' read -d "" -ra sw_vers <<< "$(awk -F'<|>' '/key|string/ {print $3}' \
+                            "/System/Library/CoreServices/SystemVersion.plist")"
+        for ((i=0;i<${#sw_vers[@]};i+=2)) {
+            case ${sw_vers[i]} in
+                ProductName)          darwin_name=${sw_vers[i+1]} ;;
+                ProductVersion)       osx_version=${sw_vers[i+1]} ;;
+                ProductBuildVersion)  osx_build=${sw_vers[i+1]}   ;;
+            esac
+        }
+    fi
+}
+
 # Get distro name
 distroName() {
     kernel_name=$(uname -s)
     case $kernel_name in
 
         Linux | GNU*)
             os=Linux
@@ -200,15 +258,15 @@
     # Get system architecture
     distroArchitecture() {
         arch=$(uname -m)
     }
 
     # Get kernel name
     kernelName() {
-        kernel=$(uname -r)
+        _kernel=$(uname -r)
     }
 
     # Get Init System
     initSystem() {
         os=$(uname -o)
         if [[ $os = Android ]]; then
             varInit="init.rc"
@@ -313,171 +371,278 @@
     }
 
     getUptime() {
         uptime=$(echo "$(uptime -p | sed 's/up//' | xargs)")
     }
 
     get_cpu() {
+        # Get CPU name.
         cpu_file="/proc/cpuinfo"
 
-        cpu="$(awk -F '\\s*: | @' \
-            '/model name|Hardware|Processor|^cpu model|chip type|^cpu type/ {
-    cpu=$2; if ($1 == "Hardware") exit } END { print cpu }' "$cpu_file")"
-
-    cpu="${cpu//(TM)/}"
-    cpu="${cpu//(tm)/}"
-    cpu="${cpu//(R)/}"
-    cpu="${cpu//(r)/}"
-    cpu="${cpu//CPU/}"
-    cpu="${cpu//Processor/}"
-    cpu="${cpu//Dual-Core/}"
-    cpu="${cpu//Quad-Core/}"
-    cpu="${cpu//Six-Core/}"
-    cpu="${cpu//Eight-Core/}"
-    cpu="${cpu//[1-9][0-9]-Core/}"
-    cpu="${cpu//[0-9]-Core/}"
-    cpu="${cpu//, * Compute Cores/}"
-    cpu="${cpu//Core / }"
-    cpu="${cpu//(\"AuthenticAMD\"*)/}"
-    cpu="${cpu//with Radeon * Graphics/}"
-    cpu="${cpu//with AMD Radeon * Graphics/}"
-    cpu="${cpu//, altivec supported/}"
-    cpu="${cpu//FPU*/}"
-    cpu="${cpu//Chip Revision*/}"
-    cpu="${cpu//Technologies, Inc/}"
-    cpu="${cpu//Core2/Core 2}"
-
-    cores=$(awk '/^core id/&&!a[$0]++{++i} END {print i}' "$cpu_file")
-    cores="${cores//[[:space:]]/}"
-
-    speed="$(lscpu | grep -e "Model name" -e "CPU max MHz" -e "CPU(s)" -m 5 | tail -1 | cut -d ":" -f 2 | cut -d "." -f 1 | xargs)"
-    speed="${speed//[[:space:]]/}"
-
-    if ((speed < 1000)); then
-        cpu="$cpu($cores) @${speed}MHz"
-        # cpu="$cpu($cores) cores"
-    else
-        [[ "$speed_shorthand" == "on" ]] && speed="$((speed / 100))"
-        speed="${speed:0:1}.${speed:1}"
-        cpu="$cpu($cores) @${speed}GHz"
-        # cpu="$cpu($cores) cores"
-    fi
+        case $kernel_machine in
+            "frv" | "hppa" | "m68k" | "openrisc" | "or"* | "powerpc" | "ppc"* | "sparc"*)
+                cpu="$(awk -F':' '/^cpu\t|^CPU/ {printf $2; exit}' "$cpu_file")"
+                ;;
 
-}
+            "s390"*)
+                cpu="$(awk -F'=' '/machine/ {print $4; exit}' "$cpu_file")"
+                ;;
 
-get_gpu() {
-    gpu_cmd="$(lspci -mm |
-        awk -F '\"|\" \"|\\(' \
-            '/"Display|"3D|"VGA/ {
+            "ia64" | "m32r")
+                cpu="$(awk -F':' '/model/ {print $2; exit}' "$cpu_file")"
+                [[ -z "$cpu" ]] && cpu="$(awk -F':' '/family/ {printf $2; exit}' "$cpu_file")"
+                ;;
+
+            *)
+                cpu="$(awk -F '\\s*: | @' \
+                    '/model name|Hardware|Processor|^cpu model|chip type|^cpu type/ {
+            cpu=$2; if ($1 == "Hardware") exit } END { print cpu }' "$cpu_file")"
+                ;;
+        esac
+
+        speed_dir="/sys/devices/system/cpu/cpu0/cpufreq"
+        speed_type="bios_limit"
+
+        # Select the right temperature file.
+        for temp_dir in /sys/class/hwmon/*; do
+            [[ "$(< "${temp_dir}/name")" =~ (cpu_thermal|coretemp|fam15h_power|k10temp) ]] && {
+                temp_dirs=("$temp_dir"/temp*_input)
+                temp_dir=${temp_dirs[0]}
+                break
+            }
+        done
+
+        # Get CPU speed.
+        if [[ -d "$speed_dir" ]]; then
+            # Fallback to bios_limit if $speed_type fails.
+            speed="$(< "${speed_dir}/${speed_type}")" ||\
+                speed="$(< "${speed_dir}/bios_limit")" ||\
+                speed="$(< "${speed_dir}/scaling_max_freq")" ||\
+                speed="$(< "${speed_dir}/cpuinfo_max_freq")"
+            speed="$((speed / 1000))"
+
+        else
+            case $kernel_machine in
+                "sparc"*)
+                    # SPARC systems use a different file to expose clock speed information.
+                    speed_file="/sys/devices/system/cpu/cpu0/clock_tick"
+                    speed="$(($(< "$speed_file") / 1000000))"
+                    ;;
+
+                *)
+                    speed="$(awk -F ': |\\.' '/cpu MHz|^clock/ {printf $2; exit}' "$cpu_file")"
+                    speed="${speed/MHz}"
+                    ;;
+            esac
+        fi
+
+        # Get CPU temp.
+        [[ -f "$temp_dir" ]] && deg="$(($(< "$temp_dir") * 100 / 10000))"
+
+        # Get CPU cores.
+        cpu_cores="physical"
+        case $kernel_machine in
+            "sparc"*)
+                case $cpu_cores in
+                        # SPARC systems doesn't expose detailed topology information in
+                        # /proc/cpuinfo so I have to use lscpu here.
+                    "logical" | "on")
+                        cores="$(lscpu | awk -F ': *' '/^CPU\(s\)/ {print $2}')"
+                        ;;
+                    "physical")
+                        cores="$(lscpu | awk -F ': *' '/^Core\(s\) per socket/ {print $2}')"
+                        sockets="$(lscpu | awk -F ': *' '/^Socket\(s\)/ {print $2}')"
+                        cores="$((sockets * cores))"
+                        ;;
+                esac
+                ;;
+
+            *)
+                case $cpu_cores in
+                    "logical" | "on")
+                        cores="$(grep -c "^processor" "$cpu_file")"
+                        ;;
+                    "physical")
+                        cores="$(awk '/^core id/&&!a[$0]++{++i} END {print i}' "$cpu_file")"
+                        ;;
+                esac
+                ;;
+        esac
+        # Remove un-needed patterns from cpu output.
+        cpu="${cpu//(TM)}"
+        cpu="${cpu//(tm)}"
+        cpu="${cpu//(R)}"
+        cpu="${cpu//(r)}"
+        cpu="${cpu//CPU}"
+        cpu="${cpu//Processor}"
+        cpu="${cpu//Dual-Core}"
+        cpu="${cpu//Quad-Core}"
+        cpu="${cpu//Six-Core}"
+        cpu="${cpu//Eight-Core}"
+        cpu="${cpu//[1-9][0-9]-Core}"
+        cpu="${cpu//[0-9]-Core}"
+        cpu="${cpu//, * Compute Cores}"
+        cpu="${cpu//Core / }"
+        cpu="${cpu//(\"AuthenticAMD\"*)}"
+        cpu="${cpu//with Radeon * Graphics}"
+        cpu="${cpu//, altivec supported}"
+        cpu="${cpu//FPU*}"
+        cpu="${cpu//Chip Revision*}"
+        cpu="${cpu//Technologies, Inc}"
+        cpu="${cpu//Core2/Core 2}"
+
+        # Trim spaces from core and speed output
+        cores="${cores//[[:space:]]}"
+        speed="${speed//[[:space:]]}"
+
+        # Remove CPU brand from the output.
+        if [[ "$cpu_brand" == "off" ]]; then
+            cpu="${cpu/AMD }"
+            cpu="${cpu/Intel }"
+            cpu="${cpu/Core? Duo }"
+            cpu="${cpu/Qualcomm }"
+        fi
+
+        # Add CPU cores to the output.
+        [[ "$cpu_cores" != "off" && "$cores" ]] && \
+            case $os in
+            "Mac OS X"|"macOS") cpu="${cpu/@/(${cores}) @}" ;;
+            *)                  cpu="$cpu ($cores)" ;;
+        esac
+
+        # Add CPU speed to the output.
+        speed_shorthand="on"
+        if [[ "$cpu_speed" != "off" && "$speed" ]]; then
+            if (( speed < 1000 )); then
+                cpu="$cpu @ ${speed}MHz"
+            else
+                [[ "$speed_shorthand" == "on" ]] && speed="$((speed / 100))"
+                speed="${speed:0:1}.${speed:1}"
+                cpu="$cpu @ ${speed}GHz"
+            fi
+        fi
+        _cpu="$cpu"
+    }
+
+    get_gpu() {
+        gpu_cmd="$(lspci -mm |
+            awk -F '\"|\" \"|\\(' \
+                '/"Display|"3D|"VGA/ {
                                   a[$0] = $1 " " $3 " " ($(NF-1) ~ /^$|^Device [[:xdigit:]]+$/ ? $4 : $(NF-1))
                               }
                               END { for (i in a) {
                                   if (!seen[a[i]]++) {
                                       sub("^[^ ]+ ", "", a[i]);
                                       print a[i]
                                   }
-        }}')"
-        IFS=$'\n' read -d "" -ra gpus <<<"$gpu_cmd"
+            }}')"
+            IFS=$'\n' read -d "" -ra gpus <<<"$gpu_cmd"
 
-        [[ "${gpus[0]}" == *Intel* && "${gpus[1]}" == *Intel* ]] && unset -v "gpus[0]"
+            [[ "${gpus[0]}" == *Intel* && "${gpus[1]}" == *Intel* ]] && unset -v "gpus[0]"
 
-        for gpu in "${gpus[@]}"; do
-            [[ "$gpu_type" == "dedicated" && "$gpu" == *Intel* ]] ||
-            [[ "$gpu_type" == "integrated" && ! "$gpu" == *Intel* ]] &&
-            {
-                unset -v gpu
-                continue
-            }
+            for gpu in "${gpus[@]}"; do
+                [[ "$gpu_type" == "dedicated" && "$gpu" == *Intel* ]] ||
+                [[ "$gpu_type" == "integrated" && ! "$gpu" == *Intel* ]] &&
+                {
+                    unset -v gpu
+                    continue
+                }
+
+                case $gpu in
+                    *"Advanced"*)
+                        brand="${gpu/*AMD*ATI*/AMD ATI}"
+                        brand="${brand:-${gpu/*AMD*/AMD}}"
+                        brand="${brand:-${gpu/*ATI*/ATi}}"
+
+                        gpu="${gpu/\[AMD\/ATI\] /}"
+                        gpu="${gpu/\[AMD\] /}"
+                        gpu="${gpu/OEM /}"
+                        gpu="${gpu/Advanced Micro Devices, Inc./}"
+                        gpu="${gpu/*\[/}"
+                        gpu="${gpu/\]*/}"
+                        gpu="$brand $gpu"
+                        ;;
 
-            case $gpu in
-                *"Advanced"*)
-                    brand="${gpu/*AMD*ATI*/AMD ATI}"
-                    brand="${brand:-${gpu/*AMD*/AMD}}"
-                    brand="${brand:-${gpu/*ATI*/ATi}}"
-
-                    gpu="${gpu/\[AMD\/ATI\] /}"
-                    gpu="${gpu/\[AMD\] /}"
-                    gpu="${gpu/OEM /}"
-                    gpu="${gpu/Advanced Micro Devices, Inc./}"
-                    gpu="${gpu/*\[/}"
-                    gpu="${gpu/\]*/}"
-                    gpu="$brand $gpu"
-                    ;;
+                    *"NVIDIA"*)
+                        gpu="${gpu/*\[/}"
+                        gpu="${gpu/\]*/}"
+                        gpu="NVIDIA $gpu"
+                        ;;
 
-                *"NVIDIA"*)
-                    gpu="${gpu/*\[/}"
-                    gpu="${gpu/\]*/}"
-                    gpu="NVIDIA $gpu"
-                    ;;
+                    *"Intel"*)
+                        gpu="${gpu/*Intel/Intel}"
+                        gpu="${gpu/\(R\)/}"
+                        gpu="${gpu/Corporation/}"
+                        gpu="${gpu/ \(*/}"
+                        gpu="${gpu/Integrated Graphics Controller/}"
+                        gpu="${gpu/*Xeon*/Intel HD Graphics}"
 
-                *"Intel"*)
-                    gpu="${gpu/*Intel/Intel}"
-                    gpu="${gpu/\(R\)/}"
-                    gpu="${gpu/Corporation/}"
-                    gpu="${gpu/ \(*/}"
-                    gpu="${gpu/Integrated Graphics Controller/}"
-                    gpu="${gpu/*Xeon*/Intel HD Graphics}"
+                        [[ -z "$(trim "$gpu")" ]] && gpu="Intel Integrated Graphics"
+                        ;;
 
-                    [[ -z "$(trim "$gpu")" ]] && gpu="Intel Integrated Graphics"
-                    ;;
+                    *"MCST"*)
+                        gpu="${gpu/*MCST*MGA2*/MCST MGA2}"
+                        ;;
 
-                *"MCST"*)
-                    gpu="${gpu/*MCST*MGA2*/MCST MGA2}"
-                    ;;
+                    *"VirtualBox"*)
+                        gpu="VirtualBox Graphics Adapter"
+                        ;;
 
-                *"VirtualBox"*)
-                    gpu="VirtualBox Graphics Adapter"
-                    ;;
+                    *) continue ;;
+                esac
+                gpu=$(echo "$gpu" | xargs)
+                if [[ "$gpu" != "" ]]; then
+                    _gpu="$_gpu 󰭯 $gpu"
+                else
+                    _gpu="NA"
+                fi
+            done
 
-                *) continue ;;
-            esac
-            gpu=$(echo "$gpu" | xargs)
-            _gpu=$(echo -e "$_gpu 󰭯 $gpu")
-        done
+            return
+        }
 
-        return
-    }
+        trim() {
+            set -f
+            # shellcheck disable=2048,2086
+            set -- $*
+            printf '%s\n' "${*//[[:space:]]/}"
+            set +f
+        }
 
-    trim() {
-        set -f
-        # shellcheck disable=2048,2086
-        set -- $*
-        printf '%s\n' "${*//[[:space:]]/}"
-        set +f
-    }
-
-    dist="NA"
-    arch=""
-    varInit=""
-    kernel="NA"
-    varPkg="NA"
-    shell="NA"
-    varWm="NA"
-    uptime="NA"
-    cpu="NA"
-    _gpu="NA"
-    storage="NA"
-    mem="NA"
-
-    distroName
-    distroArchitecture
-    initSystem
-    kernelName
-    pkgsTotal
-    defaultShell
-    storageInfo
-    memoryUsage
-    de_WM
-    getUptime
-    get_cpu
-    get_gpu
-
-    echo "OS : $dist $arch [$varInit]"
-    echo "Kernel : $kernel"
-    echo "Packages : $varPkg"
-    echo "Shell : $shell"
-    echo "DE/WM : $varWm"
-    echo "Uptime : $uptime"
-    echo "CPU : $cpu"
-    echo "GPU : $_gpu"
-    echo "Storage : $storage"
-    echo "Memory : $mem"
+        dist="NA"
+        arch=""
+        varInit=""
+        kernel="NA"
+        varPkg="NA"
+        shell="NA"
+        varWm="NA"
+        uptime="NA"
+        cpu="NA"
+        _gpu=""
+        storage="NA"
+        mem="NA"
+
+        cache_uname
+        get_kernel
+        distroName
+        distroArchitecture
+        initSystem
+        kernelName
+        pkgsTotal
+        defaultShell
+        storageInfo
+        memoryUsage
+        de_WM
+        getUptime
+        get_cpu
+        get_gpu
+
+        echo "OS : $dist $arch [$varInit]"
+        echo "Kernel : $_kernel"
+        echo "Packages : $varPkg"
+        echo "Shell : $shell"
+        echo "DE/WM : $varWm"
+        echo "Uptime : $uptime"
+        echo "CPU : $_cpu"
+        echo "GPU : $_gpu"
+        echo "Storage : $storage"
+        echo "Memory : $mem"
```

### Comparing `xhibit-9.7.0/Exhibition/sysinfo.py` & `xhibit-9.8.0/Exhibition/sysinfo.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/LICENSE` & `xhibit-9.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/PKG-INFO` & `xhibit-9.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.7.0
+Version: 9.8.0
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `xhibit-9.7.0/README.md` & `xhibit-9.8.0/README.md`

 * *Files identical despite different names*

### Comparing `xhibit-9.7.0/setup.py` & `xhibit-9.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xhibit",
-    version="9.7.0",
+    version="9.8.0",
     author="glowfi",
     description="A python script to exhibit your ascii arts and sytem specs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/glowfi/xhibit",
     classifiers=[
```

### Comparing `xhibit-9.7.0/xhibit.egg-info/PKG-INFO` & `xhibit-9.8.0/xhibit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.7.0
+Version: 9.8.0
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

