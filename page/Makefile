ARCHS = arm64 armv7
TARGET = iphone:clang:9.2:latest

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = Page
Page_FILES = Tweak.xm

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 SpringBoard"
