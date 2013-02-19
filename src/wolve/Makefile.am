bin_PROGRAMS = wolve

wolve_SOURCES = \
WolveEngine.cpp \
WolveMain.cpp \
WolvePlayer.cpp \
WolveProgram.cpp \
WolveSearch.cpp \
WolveTimeControl.cpp

noinst_HEADERS = \
WolveEngine.hpp \
WolvePlayer.hpp \
WolveProgram.hpp \
WolveSearch.hpp \
WolveTimeControl.hpp

wolve_LDADD = \
../commonengine/libcommonengine.a \
../solver/libsolver.a \
../book/libbook.a \
../hex/libhex.a \
../util/libutil.a \
$(FUEGO_BUILD)/smartgame/libfuego_smartgame.a \
$(FUEGO_BUILD)/gtpengine/libfuego_gtpengine.a \
$(DB_LIBS) \
$(BOOST_DATE_TIME_LIBS) \
$(BOOST_FILESYSTEM_LIBS) \
$(BOOST_PROGRAM_OPTIONS_LIBS) \
$(BOOST_SYSTEM_LIBS) \
$(BOOST_THREAD_LIBS)

wolve_DEPENDENCIES = \
../util/libutil.a \
../hex/libhex.a \
../book/libbook.a \
../solver/libsolver.a \
../commonengine/libcommonengine.a \
$(FUEGO_BUILD)/smartgame/libfuego_smartgame.a \
$(FUEGO_BUILD)/gtpengine/libfuego_gtpengine.a

wolve_LDFLAGS = \
$(BOOST_DATE_TIME_LDFLAGS) \
$(BOOST_FILESYSTEM_LDFLAGS) \
$(BOOST_PROGRAM_OPTIONS_LDFLAGS) \
$(BOOST_SYSTEM_LDFLAGS) \
$(BOOST_THREAD_LDFLAGS)

wolve_CPPFLAGS = \
$(BOOST_CPPFLAGS) \
-I$(FUEGO_ROOT)/smartgame \
-I$(FUEGO_ROOT)/gtpengine \
-I@top_srcdir@/src/ \
-I@top_srcdir@/src/util \
-I@top_srcdir@/src/hex \
-I@top_srcdir@/src/book \
-I@top_srcdir@/src/uct \
-I@top_srcdir@/src/solver \
-I@top_srcdir@/src/commonengine

DISTCLEANFILES = *~
