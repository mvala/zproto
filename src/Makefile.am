
AM_CFLAGS = -g
AM_CPPFLAGS = -I$(top_srcdir)/include
noinst_LTLIBRARIES = 
noinst_PROGRAMS = 
TESTS = 

# Install scripts into /usr/local/bin
zprotodir = @bindir@
zproto_DATA = \
	zproto_codec_c.gsl \
	zproto_codec_go.gsl \
	zproto_codec_java.gsl \
	zproto_server_c.gsl \
	zproto_client_c.gsl \
	zproto_bnf.gsl \
	zproto_lib.gsl \
	zproto_lib_go.gsl \
	zproto_lib_java.gsl

# Produce generated models; do this manually in src directory
code:
	gsl -q -script:zproto_codec_c zproto_example.xml
	gsl -q -script:zproto_codec_go zproto_example.xml
	gsl -q -script:zproto_codec_java zproto_example.xml
