```bash
bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$ cat socat-1.8.0.3.cygport
# socat-1.8.0.3.cygport
NAME="socat"
VERSION="1.8.0.3"
CATEGORY="net"
SRC_URI="http://www.dest-unreach.org/socat/download/${NAME}-${VERSION}.tar.gz"
HOMEPAGE="http://www.dest-unreach.org/socat/"
LICENSE="GPLv2"
REQUIRES="cygwin"

SRC_DIR="${NAME}-${VERSION}"

# Default configure options
src_configure() {
    default_configure \
        --disable-static \
        --enable-shared
}

# Installation du package
src_compile() {
    default_compile
}

# Installation dans l'arborescence Cygwin
src_install() {
    default_install
}

# Vérification du package après installation
check() {
    default_check
}

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$ nano socat-1.8.0.3.cygport

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$ cygport socat-1.8.0.3.cygport all
>>> Preparing socat-1.8.0.3.x86_64
>>> Unpacking source socat-1.8.0.3.tar.gz
>>> Preparing working source directory
>>> Compiling socat-1.8.0.3.x86_64
configure: WARNING: unrecognized options: --disable-static, --enable-shared
checking which defines needed for makedepend...
checking for gcc... gcc
checking whether the C compiler works... yes
checking for C compiler default output file name... a.exe
checking for suffix of executables... .exe
checking whether we are cross compiling... no
checking for suffix of object files... o
checking whether the compiler supports GNU C... yes
checking whether gcc accepts -g... yes
checking for gcc option to enable C11 features... none needed
checking for special C compiler options needed for large files... no
checking for _FILE_OFFSET_BITS value needed for large files... no
checking for a BSD-compatible install... /usr/bin/install -c
checking for gcc... (cached) gcc
checking whether the compiler supports GNU C... (cached) yes
checking whether gcc accepts -g... (cached) yes
checking for gcc option to enable C11 features... (cached) none needed
checking for ranlib... ranlib
checking for ar... ar
checking for stdio.h... yes
checking for stdlib.h... yes
checking for string.h... yes
checking for inttypes.h... yes
checking for stdint.h... yes
checking for strings.h... yes
checking for sys/stat.h... yes
checking for sys/types.h... yes
checking for unistd.h... yes
checking for sys/time.h... yes
checking for grep that handles long lines and -e... /usr/bin/grep
checking for egrep... /usr/bin/grep -E
checking for stdbool.h... yes
checking for inttypes.h... (cached) yes
checking for sys/wait.h that is POSIX.1 compatible... yes
checking for fcntl.h... yes
checking for limits.h... yes
checking for strings.h... (cached) yes
checking for sys/param.h... yes
checking for sys/ioctl.h... yes
checking for sys/time.h... (cached) yes
checking for syslog.h... yes
checking for unistd.h... (cached) yes
checking for pwd.h... yes
checking for grp.h... yes
checking for stdint.h... (cached) yes
checking for sys/types.h... (cached) yes
checking for poll.h... yes
checking for sys/poll.h... yes
checking for sys/socket.h... yes
checking for sys/uio.h... yes
checking for sys/stat.h... (cached) yes
checking for netdb.h... yes
checking for sys/un.h... yes
checking for pty.h... yes
checking for netinet/in.h... yes
checking for netinet/in_systm.h... yes
checking for netinet/ip.h... yes
checking for netinet/tcp.h... yes
checking for net/if.h... yes
checking for arpa/nameser.h... yes
checking for sys/types.h... (cached) yes
checking for netinet/in.h... (cached) yes
checking for arpa/nameser.h... (cached) yes
checking for netdb.h... (cached) yes
checking for resolv.h... yes
checking for termios.h... yes
checking for linux/if_tun.h... no
checking for net/if_dl.h... no
checking for linux/types.h... no
checking for linux/errqueue.h... no
checking for sys/utsname.h... yes
checking for sys/select.h... yes
checking for sys/file.h... yes
checking for util.h... no
checking for bsd/libutil.h... no
checking for libutil.h... no
checking for stropts.h... no
checking for regex.h... yes
checking for linux/fs.h... no
checking for linux/ext2_fs.h... no
checking for setgrent... yes
checking for getgrent... yes
checking for endgrent... yes
checking for getgrouplist... yes
checking for cfmakeraw... yes
checking for library containing res_9_init... no
checking for hstrerror... yes
checking for gethostent... no
checking for gethostent in -lnsl... no
checking for setsockopt... yes
checking for hstrerror prototype... yes
checking for getprotobynumber_r() variant...  /*  */
checking whether to include help... yes
checking whether to include transfer statistics... yes
checking whether to include STDIO support... yes
checking whether to include FD-number support... yes
checking whether to include direct file support... yes
checking whether to include direct create support... yes
checking whether to include gopen support... yes
checking whether to include explicit pipe support... yes
checking whether to include explicit socketpair support... yes
checking whether to include explicit termios support... yes
checking whether to include UNIX socket support... yes
checking whether to include abstract UNIX socket support... no
checking whether to include IPv4 support... yes
checking whether to include IPv6 support... yes
checking for netinet/ip6.h... yes
checking for netinet6/in6.h... no
checking if __APPLE_USE_RFC_2292 is helpful... no
checking if including netinet/in.h suffices... yes
checking whether to include raw IP support... yes
checking whether to include generic socket support... yes
checking whether to include generic network interface support... yes
checking whether to include TCP support... yes
checking whether to include UDP support... yes
checking whether to include UDP-Lite support... yes
checking for IPPROTO_UDPLITE... no
checking whether to include SCTP support... yes
checking for IPPROTO_SCTP... no
configure: WARNING: IPPROTO_SCTP undefined, disabling SCTP support
checking whether to include DCCP support... yes
checking for netinet/dccp.h... no
checking for linux/dccp.h... no
checking for IPPROTO_DCCP... no
checking whether to include vsock support... yes
checking for linux/vm_sockets.h... no
configure: WARNING: include file linux/vm_sockets.h not found, disabling vsock
checking whether to include Linux namespaces support... NO
checking whether to include listen support... yes
checking whether to include POSIX MQ support... yes
checking for mqueue.h... yes
configure: WARNING: POSIX MQ currently implemented for Linux only
checking whether to include socks4 support... yes
checking whether to include socks4a support... yes
checking whether to include socks5 support... yes
checking whether to include proxy connect support... yes
checking whether to include exec support... yes
checking whether to include system (shell) support... yes
checking whether to include shell invocation support... yes
checking whether to include pty address support... yes
checking whether to include fs attributes support... yes
checking whether to include readline support... yes
checking for usable readline in default location... yes
checking whether to include openssl support... yes
configure: checking for components of OpenSSL
configure: checked for openssl/ssl.h... yes
checking for libssl... yes
checking for OPENSSL_init_ssl... yes
checking for SSL_library_init... no
checking for OPENSSL_INIT_new... yes
checking for OPENSSL_INIT_SETTINGS... no
checking whether to include OpenSSL method option... no
checking whether to include undocumented resolver related options... yes
checking whether to include deprecated resolver option... no
checking whether to include openssl fips support... no
checking whether to include tun/tap address support... yes
configure: WARNING: include file linux/if_tun.h not found
checking for netinet/if_ether.h... no
configure: WARNING: include file netinet/if_ether.h not found, disabling interface
checking whether to include system call tracing... yes
checking whether to include file descriptor analyzer... yes
checking whether to include retry support... yes
checking whether to include devtests support... no
checking included message level... debug
checking default IP version... "0"
checking for an ANSI C-conforming const... yes
checking how to run the C preprocessor... gcc -E
checking for uid_t in sys/types.h... yes
checking for mode_t... yes
checking for off_t... yes
checking for pid_t... yes
checking for size_t... yes
checking for struct stat.st_blksize... yes
checking for struct stat.st_blocks... yes
checking for struct stat.st_rdev... yes
checking for nanosleep... yes
checking whether gcc needs -traditional... no
checking for working memcmp... yes
checking return type of signal handlers... void
checking for strftime... yes
checking for putenv... yes
checking for select... yes
checking for pselect... yes
checking for poll... yes
checking for socket... yes
checking for strtod... yes
checking for strtol... yes
checking for strtoul... yes
checking for uname... yes
checking for getpgid... yes
checking for getsid... yes
checking for gethostbyname... yes
checking for getaddrinfo... yes
checking for getprotobynumber... yes
checking for setgroups... yes
checking for inet_aton... yes
checking for grantpt... yes
checking for unlockpt... yes
checking for cfsetispeed... yes
checking for cfgetispeed... yes
checking for cfsetospeed... yes
checking for cfgetospeed... yes
checking for posix_memalign prototype... yes
checking for strdup prototype... yes
checking for strerror prototype... yes
checking for strstr prototype... yes
checking for getipnodebyname prototype... no
checking for strndup prototype... yes
checking for memrchr prototype... yes
checking for if_indextoname prototype... yes
checking for ptsname prototype... yes
checking for long long... yes
checking for sig_atomic_t... yes
checking for bool... yes
checking for socklen_t... yes
checking for struct stat64... no
checking for off64_t... no
checking for sighandler_t... yes
checking for uint8_t... yes
checking for uint16_t... yes
checking for uint32_t... yes
checking for uint64_t... yes
checking for fdset->fds_bits... yes
checking for struct termios . c_ispeed... yes
checking for struct termios . c_ospeed... yes
checking for sa_family_t... yes
checking for struct sock_extended_err... no
checking for struct sigaction.sa_sigaction... yes
checking if _SVID3 is helpful... no
checking if _XPG4_2 is helpful... no
checking for struct timespec... yes
checking for struct linger... yes
checking for struct ip... yes
checking for struct ip_mreq... yes
checking for struct ip_mreqn... no
checking for struct ipv6_mreq... yes
checking for struct ip_mreq_source... no
checking for struct group_source_req... yes
checking for struct ifreq... yes
checking for struct ifreq.ifr_index... no
checking for struct ifreq.ifr_ifindex... yes
checking for struct sockaddr.sa_len... no
checking for component names of sockaddr_in6... s6_addr
checking for struct iovec... yes
checking for struct msghdr.msg_control... yes
checking for struct msghdr.msg_controllen... yes
checking for struct msghdr.msgflags... yes
checking for struct cmsghdr... yes
checking for struct in_pktinfo... yes
checking for ipi_spec_dst in struct in_pktinfo... no
checking for struct in6_pktinfo... yes
checking for struct tpacket_auxdata... no
checking for tp_vlan_tpid in struct tpacket_auxdata... no
checking for struct ip.ip_hl... yes
checking for sigaction... yes
checking for stat64... no
checking for fstat64... no
checking for lstat64... no
checking for lseek64... no
checking for truncate64... no
checking for ftruncate64... no
checking for strtoll... yes
checking for hstrerror... (cached) yes
checking for inet_ntop... yes
checking for openpty... yes
checking for openpty in -lbsd... no
checking for openpty in -lutil... yes
checking for gettimeofday prototype... yes
checking for clock_gettime... yes
checking for getresuid... no
checking for getresgid... no
checking for flock... yes
checking for setenv... yes
checking for unsetenv... yes
checking for TLS_client_method... yes
checking for TLS_server_method... yes
checking for DTLS_client_method... yes
checking for DTLS_server_method... yes
checking for SSL_CTX_set_default_verify_paths... yes
checking for RAND_egd... no
checking for RAND_egd in -lcrypt... no
checking for DH_set0_pqg... yes
checking for ASN1_STRING_get0_data... yes
checking for RAND_status... yes
checking for SSL_CTX_clear_mode... no
checking for SSL_set_tlsext_host_name... no
checking for SSL_CTX_set_tlsext_max_fragment_length... yes
checking if SSL_CTX_set_max_send_fragment exists... yes
checking for SSL_library_init... (cached) no
checking for ERR_error_string... yes
checking for type EC_KEY... yes
checking if snprintf conforms to C99... yes
checking if printf has Z modifier... no
checking shift offset of CRDLY... 7
checking shift offset of TABDLY... 11
checking shift offset of CSIZE... 4
configure: using code run method to find basic types
checking for equivalent simple type of uint16_t... 2 /* unsigned short */
checking for equivalent simple type of uint32_t... 4 /* unsigned int */
checking for equivalent simple type of uint64_t... 6 /* unsigned long */
checking for equivalent simple type of int16_t... 1 /* short */
checking for equivalent simple type of int32_t... 3 /* int */
checking for equivalent simple type of int64_t... 5 /* long */
checking for equivalent simple type of size_t... 6 /* unsigned long */
checking for equivalent simple type of mode_t... 4 /* unsigned int */
checking for equivalent simple type of pid_t... 3 /* int */
checking for equivalent simple type of uid_t... 4 /* unsigned int */
checking for equivalent simple type of gid_t... 4 /* unsigned int */
checking for equivalent simple type of time_t... 5 /* long */
checking for equivalent simple type of socklen_t... 3 /* int */
checking for equivalent simple type of off_t... 5 /* long */
checking for equivalent simple type of off64_t... 0 /* unknown */
checking for equivalent simple type of dev_t... 4 /* unsigned int */
checking for equivalent simple type of speed_t... 4 /* unsigned int */
checking for basic type of struct stat.st_ino... 6 /* unsigned long */
checking for basic type of struct stat.st_nlink... 2 /* unsigned short */
checking for basic type of struct stat.st_size... 5 /* long */
checking for basic type of struct stat.st_blksize... 3 /* int */
checking for basic type of struct stat.st_blocks... 5 /* long */
checking for basic type of struct timeval.tv_usec... 5 /* long */
checking for basic type of struct timespec.tv_nsec... 5 /* long */
checking for basic type of struct rlimit.rlim_max... 6 /* unsigned long */
checking for basic type of struct cmsghdr.cmsg_len... 6 /* unsigned long */
checking for /dev/ptmx... yes
checking for /proc... yes
checking for /proc/*/fd... yes
checking for /proc/*/path... no
checking for d_type in struct dirent... yes
checking for _res.retrans... yes
checking for _res.retry... yes
checking for _res.nsaddr_list... yes
checking whether to include libwrap support... yes
checking for components of libwrap... configure: checked for tcpd.h... yes
checking for libwrap... yes
checking for hosts_allow_table... yes
checking for declaration of environ... yes
checking for var environ... yes
configure: creating ./config.status
config.status: creating Makefile
config.status: creating config.h
configure: WARNING: unrecognized options: --disable-static, --enable-shared
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o socat.o socat.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioinitialize.o xioinitialize.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xiohelp.o xiohelp.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioparam.o xioparam.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xiodiag.o xiodiag.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioopen.o xioopen.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioopts.o xioopts.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xiosignal.o xiosignal.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xiosigchld.o xiosigchld.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioread.o xioread.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xiowrite.o xiowrite.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xiolayer.o xiolayer.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioshutdown.o xioshutdown.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioclose.o xioclose.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xioexit.o xioexit.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-process.o xio-process.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-fd.o xio-fd.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-fdnum.o xio-fdnum.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-stdio.o xio-stdio.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-pipe.o xio-pipe.c
xio-pipe.c: Dans la fonction « xio_chk_pipesz »:
xio-pipe.c:203:13: attention: variable inutilisée « pipesz » [-Wunused-variable]
  203 |         int pipesz;
      |             ^~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-socketpair.o xio-socketpair.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-gopen.o xio-gopen.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-creat.o xio-creat.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-file.o xio-file.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-named.o xio-named.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-socket.o xio-socket.c
xio-socket.c: Dans la fonction « xiolog_ancillary_socket »:
xio-socket.c:1800:20: attention: variable inutilisée « tv » [-Wunused-variable]
 1800 |    struct timeval *tv;
      |                    ^~
Dans le fichier inclus depuis /usr/include/string.h:180,
                 depuis sysincludes.h:26,
                 depuis xiosysincludes.h:11,
                 depuis xio-socket.c:8:
Dans la fonction « __strncpy_ichk »,
    mis en ligne depuis « xiobind » à xio-socket.c:2181:6:
/usr/include/ssp/string.h:93:1: attention: « __builtin_strncpy » la limite spécifiée 108 est égale à la taille de la destination [-Wstringop-truncation]
   93 | __ssp_bos_icheck3_restrict(strncpy, char *, const char *)
      | ^~~~~~~~~~~~~~~~~~~~~~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-interface.o xio-interface.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-listen.o xio-listen.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-unix.o xio-unix.c
Dans le fichier inclus depuis /usr/include/string.h:180,
                 depuis sysincludes.h:26,
                 depuis xiosysincludes.h:11,
                 depuis xio-unix.c:7:
Dans la fonction « __strncpy_ichk »,
    mis en ligne depuis « xiosetunix » à xio-unix.c:101:4:
/usr/include/ssp/string.h:93:1: attention: « __builtin_strncpy » la limite spécifiée 108 est égale à la taille de la destination [-Wstringop-truncation]
   93 | __ssp_bos_icheck3_restrict(strncpy, char *, const char *)
      | ^~~~~~~~~~~~~~~~~~~~~~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-vsock.o xio-vsock.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-ip.o xio-ip.c
xio-ip.c: Dans la fonction « xiolog_ancillary_ip »:
xio-ip.c:957:9: attention: variable inutilisée « scratch2 » [-Wunused-variable]
  957 |    char scratch2[16];
      |         ^~~~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-ip4.o xio-ip4.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-ip6.o xio-ip6.c
Dans le fichier inclus depuis /usr/include/string.h:180,
                 depuis sysincludes.h:26,
                 depuis xiosysincludes.h:11,
                 depuis xio-ip6.c:7:
Dans la fonction « __strncpy_ichk »,
    mis en ligne depuis « xiotype_ip6_join_source_group » à xio-ip6.c:580:4:
/usr/include/ssp/string.h:93:1: attention: la sortie de « __builtin_strncpy » peut être tronquée en copiant 44 octets depuis une chaîne de longueur 511 [-Wstringop-truncation]
   93 | __ssp_bos_icheck3_restrict(strncpy, char *, const char *)
      | ^~~~~~~~~~~~~~~~~~~~~~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-ipapp.o xio-ipapp.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-tcp.o xio-tcp.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-sctp.o xio-sctp.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-dccp.o xio-dccp.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-rawip.o xio-rawip.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-posixmq.o xio-posixmq.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-socks.o xio-socks.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-socks5.o xio-socks5.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-proxy.o xio-proxy.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-udp.o xio-udp.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-udplite.o xio-udplite.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-progcall.o xio-progcall.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-exec.o xio-exec.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-system.o xio-system.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-shell.o xio-shell.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-termios.o xio-termios.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-readline.o xio-readline.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-pty.o xio-pty.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-openssl.o xio-openssl.c
xio-openssl.c: Dans la fonction « _xioopen_openssl_prepare »:
xio-openssl.c:1302:7: attention: « DH_new » est obsolète: Since OpenSSL 3.0 [-Wdeprecated-declarations]
 1302 |       dh = DH_new();
      |       ^~
Dans le fichier inclus depuis /usr/include/openssl/dsa.h:51,
                 depuis /usr/include/openssl/x509.h:37,
                 depuis /usr/include/openssl/ssl.h:31,
                 depuis sysincludes.h:200,
                 depuis xiosysincludes.h:11,
                 depuis xio-openssl.c:7:
/usr/include/openssl/dh.h:203:27: note: déclaré ici
  203 | OSSL_DEPRECATEDIN_3_0 DH *DH_new(void);
      |                           ^~~~~~
xio-openssl.c:1307:13: attention: « DH_free » est obsolète: Since OpenSSL 3.0 [-Wdeprecated-declarations]
 1307 |             DH_free(dh);
      |             ^~~~~~~
/usr/include/openssl/dh.h:204:28: note: déclaré ici
  204 | OSSL_DEPRECATEDIN_3_0 void DH_free(DH *dh);
      |                            ^~~~~~~
xio-openssl.c:1320:7: attention: « DH_set0_pqg » est obsolète: Since OpenSSL 3.0 [-Wdeprecated-declarations]
 1320 |       if (!DH_set0_pqg(dh, p, NULL, g)) {
      |       ^~
/usr/include/openssl/dh.h:259:27: note: déclaré ici
  259 | OSSL_DEPRECATEDIN_3_0 int DH_set0_pqg(DH *dh, BIGNUM *p, BIGNUM *q, BIGNUM *g);
      |                           ^~~~~~~~~~~
xio-openssl.c:1321:15: attention: « DH_free » est obsolète: Since OpenSSL 3.0 [-Wdeprecated-declarations]
 1321 |               DH_free(dh);
      |               ^~~~~~~
/usr/include/openssl/dh.h:204:28: note: déclaré ici
  204 | OSSL_DEPRECATEDIN_3_0 void DH_free(DH *dh);
      |                            ^~~~~~~
xio-openssl.c:1338:7: attention: « DH_free » est obsolète: Since OpenSSL 3.0 [-Wdeprecated-declarations]
 1338 |       DH_free(dh);
      |       ^~~~~~~
/usr/include/openssl/dh.h:204:28: note: déclaré ici
  204 | OSSL_DEPRECATEDIN_3_0 void DH_free(DH *dh);
      |                            ^~~~~~~
xio-openssl.c:1357:7: attention: « EC_KEY_new_by_curve_name » est obsolète: Since OpenSSL 3.0 [-Wdeprecated-declarations]
 1357 |       ecdh = EC_KEY_new_by_curve_name(nid);
      |       ^~~~
Dans le fichier inclus depuis /usr/include/openssl/x509.h:33:
/usr/include/openssl/ec.h:998:31: note: déclaré ici
  998 | OSSL_DEPRECATEDIN_3_0 EC_KEY *EC_KEY_new_by_curve_name(int nid);
      |                               ^~~~~~~~~~~~~~~~~~~~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-streams.o xio-streams.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-namespaces.o xio-namespaces.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-ascii.o xio-ascii.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xiolockfile.o xiolockfile.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-tcpwrap.o xio-tcpwrap.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-fs.o xio-fs.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o xio-tun.o xio-tun.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o error.o error.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o dalan.o dalan.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -c -D CC="\"gcc\"" -o procan.o ./procan.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o procan-cdefs.o procan-cdefs.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o hostan.o hostan.c
hostan.c:22:12: attention: « vsockan » déclaré « static » mais jamais défini [-Wunused-function]
   22 | static int vsockan(FILE *outfile);
      |            ^~~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o fdname.o fdname.c
fdname.c: Dans la fonction « sockname »:
fdname.c:253:8: attention: variable inutilisée « rc » [-Wunused-variable]
  253 |    int rc;
      |        ^~
fdname.c:230:31: attention: variable inutilisée « protoentp » [-Wunused-variable]
  230 |    struct protoent protoent, *protoentp;
      |                               ^~~~~~~~~
fdname.c:230:20: attention: variable inutilisée « protoent » [-Wunused-variable]
  230 |    struct protoent protoent, *protoentp;
      |                    ^~~~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o sysutils.o sysutils.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o utils.o utils.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o nestlex.o nestlex.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o vsnprintf_r.o vsnprintf_r.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o snprinterr.o snprinterr.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o filan.o filan.c
filan.c: Dans la fonction « ipan »:
filan.c:799:14: attention: variable inutilisée « optlen » [-Wunused-variable]
  799 |    socklen_t optlen = sizeof(optproto);
      |              ^~~~~~
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o sycls.o sycls.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o sslcls.o sslcls.c
sslcls.c: Dans la fonction « sycPEM_read_bio_DHparams »:
sslcls.c:456:4: attention: « PEM_read_bio_DHparams » est obsolète: Since OpenSSL 3.0 [-Wdeprecated-declarations]
  456 |    result = PEM_read_bio_DHparams(bp, x, cb, u);
      |    ^~~~~~
Dans le fichier inclus depuis /usr/include/openssl/ssl.h:36,
                 depuis sysincludes.h:200,
                 depuis sslcls.c:13:
/usr/include/openssl/pem.h:469:1: note: déclaré ici
  469 | DECLARE_PEM_rw_attr(OSSL_DEPRECATEDIN_3_0, DHparams, DH)
      | ^~~~~~~~~~~~~~~~~~~
ar r libxio.a xioinitialize.o xiohelp.o xioparam.o xiodiag.o xioopen.o xioopts.o xiosignal.o xiosigchld.o xioread.o xiowrite.o xiolayer.o xioshutdown.o xioclose.o xioexit.o xio-process.o xio-fd.o xio-fdnum.o xio-stdio.o xio-pipe.o xio-socketpair.o xio-gopen.o xio-creat.o xio-file.o xio-named.o xio-socket.o xio-interface.o xio-listen.o xio-unix.o xio-vsock.o xio-ip.o xio-ip4.o xio-ip6.o xio-ipapp.o xio-tcp.o xio-sctp.o xio-dccp.o xio-rawip.o xio-posixmq.o xio-socks.o xio-socks5.o xio-proxy.o xio-udp.o xio-udplite.o xio-progcall.o xio-exec.o xio-system.o xio-shell.o xio-termios.o xio-readline.o xio-pty.o xio-openssl.o xio-streams.o xio-namespaces.o xio-ascii.o xiolockfile.o xio-tcpwrap.o xio-fs.o xio-tun.o error.o dalan.o procan.o procan-cdefs.o hostan.o fdname.o sysutils.o utils.o nestlex.o vsnprintf_r.o snprinterr.o filan.o sycls.o sslcls.o
ar: création de libxio.a
ranlib libxio.a
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.   -o socat socat.o libxio.a -lwrap -lutil  -lreadline  -lssl -lcrypto -lcrypto
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o procan_main.o procan_main.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.   -o procan procan_main.o procan.o procan-cdefs.o hostan.o error.o sycls.o sysutils.o utils.o vsnprintf_r.o snprinterr.o -lwrap -lutil  -lreadline  -lssl -lcrypto -lcrypto
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.  -I.   -c -o filan_main.o filan_main.c
gcc -ggdb -O2 -pipe -Wall -Werror=format-security -Wp,-D_FORTIFY_SOURCE=3 -fstack-protector-strong --param=ssp-buffer-size=4 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/build=/usr/src/debug/socat-1.8.0.3 -ffile-prefix-map=/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.x86_64/src/socat-1.8.0.3=/usr/src/debug/socat-1.8.0.3 -D_GNU_SOURCE -Wall -Wno-parentheses  -DHAVE_CONFIG_H -I.   -o filan filan_main.o filan.o fdname.o error.o sycls.o sysutils.o utils.o vsnprintf_r.o snprinterr.o -lwrap -lutil  -lreadline  -lssl -lcrypto -lcrypto
>>> Installing socat-1.8.0.3.x86_64
/cygdrive/c/Users/bbrod/Downloads/socat-1.8.0.3.cygport: ligne 27: default_install : commande introuvable

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$ socat -V
socat by Gerhard Rieger and contributors - see www.dest-unreach.org
socat version 1.8.0.3 on Mar  4 2025 14:56:29
   running on CYGWIN_NT-10.0-26100 version 2025-01-29 19:46 UTC, release 3.5.7-1.x86_64, machine x86_64
features:
  #define WITH_HELP 1
  #define WITH_STATS 1
  #define WITH_STDIO 1
  #define WITH_FDNUM 1
  #define WITH_FILE 1
  #define WITH_CREAT 1
  #define WITH_GOPEN 1
  #define WITH_TERMIOS 1
  #define WITH_PIPE 1
  #define WITH_SOCKETPAIR 1
  #define WITH_UNIX 1
  #undef WITH_ABSTRACT_UNIXSOCKET
  #define WITH_IP4 1
  #define WITH_IP6 1
  #define WITH_RAWIP 1
  #define WITH_GENERICSOCKET 1
  #undef WITH_INTERFACE
  #define WITH_TCP 1
  #define WITH_UDP 1
  #undef WITH_SCTP
  #undef WITH_DCCP
  #undef WITH_UDPLITE
  #define WITH_LISTEN 1
  #undef WITH_POSIXMQ
  #define WITH_SOCKS4 1
  #define WITH_SOCKS4A 1
  #define WITH_SOCKS5 1
  #undef WITH_VSOCK
  #undef WITH_NAMESPACES
  #define WITH_PROXY 1
  #define WITH_SYSTEM 1
  #define WITH_SHELL 1
  #define WITH_EXEC 1
  #define WITH_READLINE 1
  #undef WITH_TUN
  #define WITH_PTY 1
  #define WITH_OPENSSL 1
  #undef WITH_FIPS
  #define WITH_LIBWRAP 1
  #define WITH_SYCLS 1
  #define WITH_FILAN 1
  #define WITH_RETRY 1
  #undef WITH_DEVTESTS
  #define WITH_MSGLEVEL 0 /*debug*/
  #define WITH_DEFAULT_IPV 4

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$ cat socat-1.8.0.3.
socat-1.8.0.3.cygport  socat-1.8.0.3.tar.gz   socat-1.8.0.3.x86_64/

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
$ cat socat-1.8.0.3.cygport
# socat-1.8.0.3.cygport
NAME="socat"
VERSION="1.8.0.3"
CATEGORY="net"
SRC_URI="http://www.dest-unreach.org/socat/download/${NAME}-${VERSION}.tar.gz"
HOMEPAGE="http://www.dest-unreach.org/socat/"
LICENSE="GPLv2"
REQUIRES="cygwin"

SRC_DIR="${NAME}-${VERSION}"

# Default configure options
src_configure() {
    default_configure \
        --disable-static \
        --enable-shared
}

# Installation du package
src_compile() {
    ./configure --disable-static --enable-shared
    make
}

# Installation dans l'arborescence Cygwin
src_install() {
    default_install
}

# Vérification du package après installation
check() {
    default_check
}

bbrod@DESKTOP-GZ301ZC /cygdrive/c/Users/bbrod/Downloads
```
