PKG_NAME = mediainfo
PKG_VERS = 0.7.64
PKG_EXT = tar.gz
PKG_DIST_NAME = $(PKG_NAME)_$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = http://downloads.sourceforge.net/project/mediainfo/source/$(PKG_NAME)/$(PKG_VERS)
PKG_DIR = MediaInfo/Project/GNU/CLI

DEPENDS = cross/libmediainfo

HOMEPAGE = http://sourceforge.net/projects/mediainfo/
COMMENT  = MediaInfo is a convenient unified display of the most relevant technical and tag data for video and audio files.
LICENSE  = 

PRE_CONFIGURE_TARGET = myPreConfigure
GNU_CONFIGURE = 1

CONFIGURE_ARGS = --enable-shared

include ../../mk/spksrc.cross-cc.mk

myPreConfigure:
	$(RUN) ; ./autogen
