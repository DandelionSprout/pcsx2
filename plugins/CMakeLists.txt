# Check that people use the good file
if(NOT TOP_CMAKE_WAS_SOURCED)
    message(FATAL_ERROR "
    You did not 'cmake' the good CMakeLists.txt file. Use the one in the top dir.
    It is advice to delete all wrongly generated cmake stuff => CMakeFiles & CMakeCache.txt")
endif()


if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/cdvdGigaherz" AND cdvdGigaherz)
	add_subdirectory(cdvdGigaherz/src)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/CDVDnull" AND CDVDnull)
	add_subdirectory(CDVDnull)
endif()

#if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/CDVDpeops" AND CDVDpeops)
#	add_subdirectory(CDVDpeops)
#endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/dev9null" AND dev9null)
	add_subdirectory(dev9null)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/FWnull" AND FWnull)
	add_subdirectory(FWnull)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/GSdx" AND GSdx)
	add_subdirectory(GSdx)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/GSdx_legacy" AND GSdx AND GSDX_LEGACY)
	add_subdirectory(GSdx_legacy)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/GSnull" AND GSnull)
	add_subdirectory(GSnull)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/LilyPad" AND LilyPad)
	add_subdirectory(LilyPad)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/onepad" AND onepad)
	add_subdirectory(onepad)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/PadNull" AND PadNull)
	add_subdirectory(PadNull)
endif()

# if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/PeopsSPU2" AND PeopsSPU2)
# 	add_subdirectory(PeopsSPU2)
# endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/SPU2null" AND SPU2null)
	add_subdirectory(SPU2null)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/spu2-x" AND spu2-x)
	add_subdirectory(spu2-x/src)
endif()

#if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/SSSPSXPAD" AND SSSPSXPAD)
#	add_subdirectory(SSSPSXPAD)
#endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/USBnull" AND USBnull)
	add_subdirectory(USBnull)
endif()

#if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/xpad" AND xpad)
#	add_subdirectory(xpad)
#endif()

#if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/zerogs" AND zerogs)
#	add_subdirectory(zerogs)
#endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/zzogl-pg" AND zzogl)
	add_subdirectory(zzogl-pg/opengl)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/zeropad" AND zeropad)
	add_subdirectory(zeropad)
endif()

if(EXISTS "${CMAKE_SOURCE_DIR}/plugins/zerospu2" AND zerospu2)
	add_subdirectory(zerospu2)
endif()

