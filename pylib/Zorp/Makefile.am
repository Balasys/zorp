
pkgdatadir = @ZORP_PYTHON_DIR@

pkgdata_DATA = Auth.py AuthDB.py Base.py Core.py Chainer.py Common.py \
	Dispatch.py Subnet.py Matcher.py NAT.py \
	Proxy.py Router.py Service.py Session.py \
	SockAddr.py Stream.py Zone.py Zorp.py __init__.py \
	Globals.py Cache.py Resolver.py Stack.py Config.py \
	Keybridge.py Util.py Rule.py Exceptions.py \
	Encryption.py Detector.py \
	Instance.py InstancesConf.py \
	ResolverCache.py FileLock.py

pkgdata_DATA += \
	APR.py \
	AnyPy.py \
	Finger.py \
	Ftp.py \
	Http.py \
	Plug.py \
	Pop3.py \
	Smtp.py \
	Telnet.py \
	Whois.py


Config.py: Config_.py
	cp $< $@
	$(SED) -i "s#ZORP_LIBDIR#@ZORP_LIBDIR@#" $@
	$(SED) -i "s#ZORP_SBINDIR#@ZORP_SBINDIR@#" $@
	$(SED) -i "s#ZORP_SYSCONFDIR#@ZORP_SYSCONFDIR@#" $@
	$(SED) -i "s#ZORP_PIDFILEDIR#@ZORP_PIDFILEDIR@#" $@

EXTRA_DIST = $(pkgdata_DATA)
