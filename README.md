# zxing-android
zxing c++ android ndk

Android.mk fix next  

define all-cpp-files-under
$(patsubst ./%,%, \
	$(shell  find $(LOCAL_PATH)  -name "*.cpp" -and -not -name ".*"))
endef

define all-cc-files-under
$(patsubst ./%,%, \
	$(shell find $(LOCAL_PATH) -name "*.cc" -and -not -name ".*"))
endef

