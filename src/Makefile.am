#
# $Id$
#

noinst_LIBRARIES = libgateway.a

bin_PROGRAMS = wifidog \
	wdctl
 
AM_CPPFLAGS = \
	-I${top_srcdir}/libhttpd/ \
	-Wall \
	-Wextra \
	-Wno-unused-parameter
wifidog_LDADD = libgateway.a $(top_builddir)/libhttpd/libhttpd.la

wifidog_SOURCES = main.c

libgateway_a_SOURCES = commandline.c \
	conf.c \
	debug.c \
	fw_iptables.c \
	firewall.c \
	gateway.c \
	centralserver.c \
	http.c \
	auth.c \
	client_list.c \
	util.c \
	wdctl_thread.c \
	ping_thread.c \
	safe.c \
	httpd_thread.c \
	simple_http.c \
	pstring.c \
	threadpool.c \
	ipset.c \
	https_server.c \
	uvhttp_base.c \
	uvhttp_ssl_server.c \
	uvhttp_util.c \
	wd_util.c

noinst_HEADERS = commandline.h \
	common.h \
	conf.h \
	debug.h \
	fw_iptables.h \
	firewall.h \
	gateway.h \
	centralserver.h \
	http.h \
	auth.h \
	client_list.h \
	util.h \
	wdctl_thread.h \
	wdctl.h \
	ping_thread.h \
	safe.h \
	httpd_thread.h \
	simple_http.h \
	pstring.h \
	threadpool.h \
	ipset.h \
	https_server.h \
	uvhttp_base.h \
	uvhttp_internal.h \
	uvhttp_server_internal.h \
	uvhttp_ssl_server.h \
	wd_util.h

wdctl_LDADD = libgateway.a

wdctl_SOURCES = wdctl.c
