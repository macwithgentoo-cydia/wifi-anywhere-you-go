ARCHS = armv7 arm64
TARGET = iphone:clang:latest:5.0

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = WiFiEverywherePrefs
WiFiEverywherePrefs_FILES = RootListController.m
WiFiEverywherePrefs_INSTALL_PATH = /Library/PreferenceBundles
WiFiEverywherePrefs_FRAMEWORKS = UIKit
WiFiEverywherePrefs_PRIVATE_FRAMEWORKS = Preferences
WiFiEverywherePrefs_RESOURCE_DIRS = Resources
WiFiEverywherePrefs_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/bundle.mk

include $(THEOS_MAKE_PATH)/package.mk
