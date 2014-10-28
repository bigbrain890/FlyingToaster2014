# Wind River Workbench generated Makefile.
# Do not edit!!!
#
# The file ".wrmakefile" is the template used by the Wind River Workbench to
# generate the makefiles of this project. Add user-specific build targets and
# make rules only(!) in this project's ".wrmakefile" file. These will then be
# automatically dumped into the makefiles.

WIND_HOME := $(subst \,/,$(WIND_HOME))
WIND_BASE := $(subst \,/,$(WIND_BASE))
WIND_USR := $(subst \,/,$(WIND_USR))

all : pre_build main_all post_build

_clean ::
	@echo "make: removing targets and objects of `pwd`"

TRACE=0
TRACEON=$(TRACE:0=@)
TRACE_FLAG=$(TRACEON:1=)

MAKEFILE := Makefile

FLEXIBLE_BUILD := 1

BUILD_SPEC = PPC603gnu
DEBUG_MODE = 1
ifeq ($(DEBUG_MODE),1)
MODE_DIR := Debug
else
MODE_DIR := NonDebug
endif
OBJ_DIR := .
WS_ROOT_DIR := C:/WindRiver/workspace
PRJ_ROOT_DIR := $(WS_ROOT_DIR)/FlyingToasters2014



#Global Build Macros
PROJECT_TYPE = DKM
DEFINES = 
EXPAND_DBG = 0


#BuildSpec specific Build Macros
VX_CPU_FAMILY = ppc
CPU = PPC603
TOOL_FAMILY = gnu
TOOL = gnu
TOOL_PATH = 
CC_ARCH_SPEC = -mcpu=603 -mstrict-align -mno-implicit-fp -mlongcall
LIBPATH = 
LIBS = 

IDE_INCLUDES = -I$(WIND_BASE)/target/h -I$(WIND_BASE)/target/h/WPILib -I$(WIND_BASE)/target/h/wrn/coreip 

IDE_LIBRARIES = $(WIND_BASE)/target/lib/WPILib.a 

IDE_DEFINES = 



#BuildTool flags
ifeq ($(DEBUG_MODE),1)
DEBUGFLAGS_C-Compiler = -g
DEBUGFLAGS_C++-Compiler = -g
DEBUGFLAGS_Linker = -g
DEBUGFLAGS_Partial-Image-Linker = 
DEBUGFLAGS_Librarian = 
DEBUGFLAGS_Assembler = -g
else
DEBUGFLAGS_C-Compiler = -O2 -fstrength-reduce -fno-builtin
DEBUGFLAGS_C++-Compiler = -O2 -fstrength-reduce -fno-builtin
DEBUGFLAGS_Linker = -O2 -fstrength-reduce -fno-builtin
DEBUGFLAGS_Partial-Image-Linker = 
DEBUGFLAGS_Librarian = 
DEBUGFLAGS_Assembler = -O2 -fstrength-reduce -fno-builtin
endif


#Project Targets
PROJECT_TARGETS = Vision2014/$(MODE_DIR)/Vision2014.out \
	 Vision2014_partialImage/$(MODE_DIR)/Vision2014_partialImage.o


#Rules

# Vision2014
ifeq ($(DEBUG_MODE),1)
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_C-Compiler = -g
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_C++-Compiler = -g
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Linker = -g
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Partial-Image-Linker = 
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Librarian = 
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Assembler = -g
else
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_C-Compiler = -O2 -fstrength-reduce -fno-builtin
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_C++-Compiler = -O2 -fstrength-reduce -fno-builtin
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Linker = -O2 -fstrength-reduce -fno-builtin
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Partial-Image-Linker = 
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Librarian = 
Vision2014/$(MODE_DIR)/% : DEBUGFLAGS_Assembler = -O2 -fstrength-reduce -fno-builtin
endif
Vision2014/$(MODE_DIR)/% : IDE_INCLUDES = -I$(WIND_BASE)/target/h -I$(WIND_BASE)/target/h/WPILib -I$(WIND_BASE)/target/h/wrn/coreip 
Vision2014/$(MODE_DIR)/% : IDE_LIBRARIES = $(WIND_BASE)/target/lib/WPILib.a 
Vision2014/$(MODE_DIR)/% : IDE_DEFINES = 
Vision2014/$(MODE_DIR)/% : PROJECT_TYPE = DKM
Vision2014/$(MODE_DIR)/% : DEFINES = 
Vision2014/$(MODE_DIR)/% : EXPAND_DBG = 0
Vision2014/$(MODE_DIR)/% : VX_CPU_FAMILY = ppc
Vision2014/$(MODE_DIR)/% : CPU = PPC603
Vision2014/$(MODE_DIR)/% : TOOL_FAMILY = gnu
Vision2014/$(MODE_DIR)/% : TOOL = gnu
Vision2014/$(MODE_DIR)/% : TOOL_PATH = 
Vision2014/$(MODE_DIR)/% : CC_ARCH_SPEC = -mcpu=603 -mstrict-align -mno-implicit-fp -mlongcall
Vision2014/$(MODE_DIR)/% : LIBPATH = 
Vision2014/$(MODE_DIR)/% : LIBS = 
Vision2014/$(MODE_DIR)/% : OBJ_DIR := Vision2014/$(MODE_DIR)

OBJECTS_Vision2014 = Vision2014_partialImage/$(MODE_DIR)/Vision2014_partialImage.o

Vision2014/$(MODE_DIR)/Vision2014.out : $(OBJECTS_Vision2014)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@";rm -f "$@";nmppc $(OBJECTS_Vision2014) $(IDE_LIBRARIES) | tclsh $(WIND_BASE)/host/resource/hutils/tcl/munch.tcl -c ppc > $(OBJ_DIR)/ctdt.c; $(TOOL_PATH)ccppc $(DEBUGFLAGS_Linker) $(CC_ARCH_SPEC) -fdollars-in-identifiers -Wall $(ADDED_CFLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES)  -o $(OBJ_DIR)/ctdt.o -c $(OBJ_DIR)/ctdt.c; $(TOOL_PATH)ccppc -r -nostdlib -Wl,-X -T $(WIND_BASE)/target/h/tool/gnu/ldscripts/link.OUT -o "$@" $(OBJ_DIR)/ctdt.o $(OBJECTS_Vision2014) $(IDE_LIBRARIES) $(LIBPATH) $(LIBS)  $(ADDED_LIBPATH) $(ADDED_LIBS) && if [ "$(EXPAND_DBG)" = "1" ]; then plink "$@";fi

Vision2014/$(MODE_DIR)/Vision2014_compile_file : $(FILE) ;

_clean :: Vision2014/$(MODE_DIR)/Vision2014_clean

Vision2014/$(MODE_DIR)/Vision2014_clean : 
	$(TRACE_FLAG)if [ -d "Vision2014" ]; then cd "Vision2014"; rm -rf $(MODE_DIR); fi


# Vision2014_partialImage
ifeq ($(DEBUG_MODE),1)
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_C-Compiler = -g
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_C++-Compiler = -g
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Linker = -g
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Partial-Image-Linker = 
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Librarian = 
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Assembler = -g
else
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_C-Compiler = -O2 -fstrength-reduce -fno-builtin
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_C++-Compiler = -O2 -fstrength-reduce -fno-builtin
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Linker = -O2 -fstrength-reduce -fno-builtin
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Partial-Image-Linker = 
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Librarian = 
Vision2014_partialImage/$(MODE_DIR)/% : DEBUGFLAGS_Assembler = -O2 -fstrength-reduce -fno-builtin
endif
Vision2014_partialImage/$(MODE_DIR)/% : IDE_INCLUDES = -I$(WIND_BASE)/target/h -I$(WIND_BASE)/target/h/WPILib -I$(WIND_BASE)/target/h/wrn/coreip 
Vision2014_partialImage/$(MODE_DIR)/% : IDE_LIBRARIES = $(WIND_BASE)/target/lib/WPILib.a 
Vision2014_partialImage/$(MODE_DIR)/% : IDE_DEFINES = 
Vision2014_partialImage/$(MODE_DIR)/% : PROJECT_TYPE = DKM
Vision2014_partialImage/$(MODE_DIR)/% : DEFINES = 
Vision2014_partialImage/$(MODE_DIR)/% : EXPAND_DBG = 0
Vision2014_partialImage/$(MODE_DIR)/% : VX_CPU_FAMILY = ppc
Vision2014_partialImage/$(MODE_DIR)/% : CPU = PPC603
Vision2014_partialImage/$(MODE_DIR)/% : TOOL_FAMILY = gnu
Vision2014_partialImage/$(MODE_DIR)/% : TOOL = gnu
Vision2014_partialImage/$(MODE_DIR)/% : TOOL_PATH = 
Vision2014_partialImage/$(MODE_DIR)/% : CC_ARCH_SPEC = -mcpu=603 -mstrict-align -mno-implicit-fp -mlongcall
Vision2014_partialImage/$(MODE_DIR)/% : LIBPATH = 
Vision2014_partialImage/$(MODE_DIR)/% : LIBS = 
Vision2014_partialImage/$(MODE_DIR)/% : OBJ_DIR := Vision2014_partialImage/$(MODE_DIR)

Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/FlyingToasters2014.o : $(PRJ_ROOT_DIR)/FlyingToasters2014.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ADXL345_I2C.o : $(PRJ_ROOT_DIR)/WPILib/ADXL345_I2C.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ADXL345_SPI.o : $(PRJ_ROOT_DIR)/WPILib/ADXL345_SPI.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Accelerometer.o : $(PRJ_ROOT_DIR)/WPILib/Accelerometer.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogChannel.o : $(PRJ_ROOT_DIR)/WPILib/AnalogChannel.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogModule.o : $(PRJ_ROOT_DIR)/WPILib/AnalogModule.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogPotentiometer.o : $(PRJ_ROOT_DIR)/WPILib/AnalogPotentiometer.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogTrigger.o : $(PRJ_ROOT_DIR)/WPILib/AnalogTrigger.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogTriggerOutput.o : $(PRJ_ROOT_DIR)/WPILib/AnalogTriggerOutput.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/AnalogIOButton.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/AnalogIOButton.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/Button.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/Button.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ButtonScheduler.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/ButtonScheduler.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/CancelButtonScheduler.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/CancelButtonScheduler.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/DigitalIOButton.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/DigitalIOButton.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/HeldButtonScheduler.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/HeldButtonScheduler.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/InternalButton.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/InternalButton.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/JoystickButton.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/JoystickButton.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/NetworkButton.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/NetworkButton.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/PressedButtonScheduler.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/PressedButtonScheduler.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ReleasedButtonScheduler.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/ReleasedButtonScheduler.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ToggleButtonScheduler.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/ToggleButtonScheduler.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/Trigger.o : $(PRJ_ROOT_DIR)/WPILib/Buttons/Trigger.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/CANJaguar.o : $(PRJ_ROOT_DIR)/WPILib/CANJaguar.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Command.o : $(PRJ_ROOT_DIR)/WPILib/Commands/Command.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/CommandGroup.o : $(PRJ_ROOT_DIR)/WPILib/Commands/CommandGroup.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/CommandGroupEntry.o : $(PRJ_ROOT_DIR)/WPILib/Commands/CommandGroupEntry.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PIDCommand.o : $(PRJ_ROOT_DIR)/WPILib/Commands/PIDCommand.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PIDSubsystem.o : $(PRJ_ROOT_DIR)/WPILib/Commands/PIDSubsystem.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PrintCommand.o : $(PRJ_ROOT_DIR)/WPILib/Commands/PrintCommand.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Scheduler.o : $(PRJ_ROOT_DIR)/WPILib/Commands/Scheduler.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/StartCommand.o : $(PRJ_ROOT_DIR)/WPILib/Commands/StartCommand.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Subsystem.o : $(PRJ_ROOT_DIR)/WPILib/Commands/Subsystem.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitCommand.o : $(PRJ_ROOT_DIR)/WPILib/Commands/WaitCommand.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitForChildren.o : $(PRJ_ROOT_DIR)/WPILib/Commands/WaitForChildren.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitUntilCommand.o : $(PRJ_ROOT_DIR)/WPILib/Commands/WaitUntilCommand.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Compressor.o : $(PRJ_ROOT_DIR)/WPILib/Compressor.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Counter.o : $(PRJ_ROOT_DIR)/WPILib/Counter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Dashboard.o : $(PRJ_ROOT_DIR)/WPILib/Dashboard.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalInput.o : $(PRJ_ROOT_DIR)/WPILib/DigitalInput.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalModule.o : $(PRJ_ROOT_DIR)/WPILib/DigitalModule.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalOutput.o : $(PRJ_ROOT_DIR)/WPILib/DigitalOutput.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalSource.o : $(PRJ_ROOT_DIR)/WPILib/DigitalSource.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DoubleSolenoid.o : $(PRJ_ROOT_DIR)/WPILib/DoubleSolenoid.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStation.o : $(PRJ_ROOT_DIR)/WPILib/DriverStation.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStationEnhancedIO.o : $(PRJ_ROOT_DIR)/WPILib/DriverStationEnhancedIO.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStationLCD.o : $(PRJ_ROOT_DIR)/WPILib/DriverStationLCD.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Encoder.o : $(PRJ_ROOT_DIR)/WPILib/Encoder.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Error.o : $(PRJ_ROOT_DIR)/WPILib/Error.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ErrorBase.o : $(PRJ_ROOT_DIR)/WPILib/ErrorBase.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/GearTooth.o : $(PRJ_ROOT_DIR)/WPILib/GearTooth.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Gyro.o : $(PRJ_ROOT_DIR)/WPILib/Gyro.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/HiTechnicColorSensor.o : $(PRJ_ROOT_DIR)/WPILib/HiTechnicColorSensor.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/HiTechnicCompass.o : $(PRJ_ROOT_DIR)/WPILib/HiTechnicCompass.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/I2C.o : $(PRJ_ROOT_DIR)/WPILib/I2C.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/InterruptableSensorBase.o : $(PRJ_ROOT_DIR)/WPILib/InterruptableSensorBase.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/IterativeRobot.o : $(PRJ_ROOT_DIR)/WPILib/IterativeRobot.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Jaguar.o : $(PRJ_ROOT_DIR)/WPILib/Jaguar.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Joystick.o : $(PRJ_ROOT_DIR)/WPILib/Joystick.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Kinect.o : $(PRJ_ROOT_DIR)/WPILib/Kinect.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/KinectStick.o : $(PRJ_ROOT_DIR)/WPILib/KinectStick.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/LiveWindow/LiveWindow.o : $(PRJ_ROOT_DIR)/WPILib/LiveWindow/LiveWindow.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/LiveWindow/LiveWindowStatusListener.o : $(PRJ_ROOT_DIR)/WPILib/LiveWindow/LiveWindowStatusListener.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Module.o : $(PRJ_ROOT_DIR)/WPILib/Module.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/MotorSafetyHelper.o : $(PRJ_ROOT_DIR)/WPILib/MotorSafetyHelper.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Notifier.o : $(PRJ_ROOT_DIR)/WPILib/Notifier.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/OSAL/Synchronized.o : $(PRJ_ROOT_DIR)/WPILib/OSAL/Synchronized.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/OSAL/Task.o : $(PRJ_ROOT_DIR)/WPILib/OSAL/Task.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/PIDController.o : $(PRJ_ROOT_DIR)/WPILib/PIDController.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/PWM.o : $(PRJ_ROOT_DIR)/WPILib/PWM.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Preferences.o : $(PRJ_ROOT_DIR)/WPILib/Preferences.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Relay.o : $(PRJ_ROOT_DIR)/WPILib/Relay.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Resource.o : $(PRJ_ROOT_DIR)/WPILib/Resource.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/RobotBase.o : $(PRJ_ROOT_DIR)/WPILib/RobotBase.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/RobotDrive.o : $(PRJ_ROOT_DIR)/WPILib/RobotDrive.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SPI.o : $(PRJ_ROOT_DIR)/WPILib/SPI.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SafePWM.o : $(PRJ_ROOT_DIR)/WPILib/SafePWM.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SensorBase.o : $(PRJ_ROOT_DIR)/WPILib/SensorBase.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SerialPort.o : $(PRJ_ROOT_DIR)/WPILib/SerialPort.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Servo.o : $(PRJ_ROOT_DIR)/WPILib/Servo.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SimpleRobot.o : $(PRJ_ROOT_DIR)/WPILib/SimpleRobot.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SmartDashboard/SendableChooser.o : $(PRJ_ROOT_DIR)/WPILib/SmartDashboard/SendableChooser.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SmartDashboard/SmartDashboard.o : $(PRJ_ROOT_DIR)/WPILib/SmartDashboard/SmartDashboard.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Solenoid.o : $(PRJ_ROOT_DIR)/WPILib/Solenoid.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SolenoidBase.o : $(PRJ_ROOT_DIR)/WPILib/SolenoidBase.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Synchronized.o : $(PRJ_ROOT_DIR)/WPILib/Synchronized.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Talon.o : $(PRJ_ROOT_DIR)/WPILib/Talon.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Task.o : $(PRJ_ROOT_DIR)/WPILib/Task.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Timer.o : $(PRJ_ROOT_DIR)/WPILib/Timer.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Ultrasonic.o : $(PRJ_ROOT_DIR)/WPILib/Ultrasonic.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Utility.o : $(PRJ_ROOT_DIR)/WPILib/Utility.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Victor.o : $(PRJ_ROOT_DIR)/WPILib/Victor.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/AxisCamera.o : $(PRJ_ROOT_DIR)/WPILib/Vision/AxisCamera.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/AxisCameraParams.o : $(PRJ_ROOT_DIR)/WPILib/Vision/AxisCameraParams.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/BinaryImage.o : $(PRJ_ROOT_DIR)/WPILib/Vision/BinaryImage.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/ColorImage.o : $(PRJ_ROOT_DIR)/WPILib/Vision/ColorImage.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/EnumCameraParameter.o : $(PRJ_ROOT_DIR)/WPILib/Vision/EnumCameraParameter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/HSLImage.o : $(PRJ_ROOT_DIR)/WPILib/Vision/HSLImage.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/ImageBase.o : $(PRJ_ROOT_DIR)/WPILib/Vision/ImageBase.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/IntCameraParameter.o : $(PRJ_ROOT_DIR)/WPILib/Vision/IntCameraParameter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/MonoImage.o : $(PRJ_ROOT_DIR)/WPILib/Vision/MonoImage.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/PCVideoServer.o : $(PRJ_ROOT_DIR)/WPILib/Vision/PCVideoServer.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/RGBImage.o : $(PRJ_ROOT_DIR)/WPILib/Vision/RGBImage.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/Threshold.o : $(PRJ_ROOT_DIR)/WPILib/Vision/Threshold.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/AxisCamera.o : $(PRJ_ROOT_DIR)/WPILib/Vision2009/AxisCamera.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/BaeUtilities.o : $(PRJ_ROOT_DIR)/WPILib/Vision2009/BaeUtilities.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/FrcError.o : $(PRJ_ROOT_DIR)/WPILib/Vision2009/FrcError.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/TrackAPI.o : $(PRJ_ROOT_DIR)/WPILib/Vision2009/TrackAPI.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/VisionAPI.o : $(PRJ_ROOT_DIR)/WPILib/Vision2009/VisionAPI.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Watchdog.o : $(PRJ_ROOT_DIR)/WPILib/Watchdog.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTable.o : $(PRJ_ROOT_DIR)/WPILib/networktables/NetworkTable.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableConnectionListenerAdapter.o : $(PRJ_ROOT_DIR)/WPILib/networktables/NetworkTableConnectionListenerAdapter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableKeyListenerAdapter.o : $(PRJ_ROOT_DIR)/WPILib/networktables/NetworkTableKeyListenerAdapter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableListenerAdapter.o : $(PRJ_ROOT_DIR)/WPILib/networktables/NetworkTableListenerAdapter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableMode.o : $(PRJ_ROOT_DIR)/WPILib/networktables/NetworkTableMode.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableProvider.o : $(PRJ_ROOT_DIR)/WPILib/networktables/NetworkTableProvider.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableSubListenerAdapter.o : $(PRJ_ROOT_DIR)/WPILib/networktables/NetworkTableSubListenerAdapter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/AbstractNetworkTableEntryStore.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/AbstractNetworkTableEntryStore.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/NetworkTableEntry.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/NetworkTableEntry.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/NetworkTableNode.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/NetworkTableNode.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/OutgoingEntryReciever.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/OutgoingEntryReciever.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/TableKeyExistsWithDifferentTypeException.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/TableKeyExistsWithDifferentTypeException.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/TransactionDirtier.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/TransactionDirtier.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/WriteManager.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/WriteManager.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientConnectionAdapter.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/client/ClientConnectionAdapter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientConnectionState.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/client/ClientConnectionState.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientNetworkTableEntryStore.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/client/ClientNetworkTableEntryStore.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/NetworkTableClient.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/client/NetworkTableClient.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/BadMessageException.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/connection/BadMessageException.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/ConnectionMonitorThread.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/connection/ConnectionMonitorThread.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/DataIOStream.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/connection/DataIOStream.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/NetworkTableConnection.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/connection/NetworkTableConnection.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/NetworkTableServer.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/server/NetworkTableServer.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionAdapter.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/server/ServerConnectionAdapter.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionList.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/server/ServerConnectionList.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionState.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/server/ServerConnectionState.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerIncomingStreamMonitor.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/server/ServerIncomingStreamMonitor.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerNetworkTableEntryStore.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/server/ServerNetworkTableEntryStore.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/FDIOStream.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/stream/FDIOStream.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketServerStreamProvider.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/stream/SocketServerStreamProvider.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketStreamFactory.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/stream/SocketStreamFactory.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketStreams.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/stream/SocketStreams.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/thread/DefaultThreadManger.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/thread/DefaultThreadManger.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ArrayData.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/ArrayData.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ArrayEntryType.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/ArrayEntryType.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/BooleanArray.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/BooleanArray.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ComplexData.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/ComplexData.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ComplexEntryType.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/ComplexEntryType.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/DefaultEntryTypes.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/DefaultEntryTypes.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NetworkTableEntryType.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/NetworkTableEntryType.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NetworkTableEntryTypeManager.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/NetworkTableEntryTypeManager.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NumberArray.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/NumberArray.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/StringArray.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/type/StringArray.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/EOFException.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/util/EOFException.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/IOException.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/util/IOException.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/IllegalStateException.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/util/IllegalStateException.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/StringCache.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/util/StringCache.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/System.o : $(PRJ_ROOT_DIR)/WPILib/networktables2/util/System.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/tables/TableKeyNotDefinedException.o : $(PRJ_ROOT_DIR)/WPILib/tables/TableKeyNotDefinedException.cpp $(FORCE_FILE_BUILD)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc $(DEBUGFLAGS_C++-Compiler) $(CC_ARCH_SPEC) -ansi -Wall  -MD -MP -mlongcall $(ADDED_C++FLAGS) $(IDE_INCLUDES) $(ADDED_INCLUDES) -DCPU=$(CPU) -DTOOL_FAMILY=$(TOOL_FAMILY) -DTOOL=$(TOOL) -D_WRS_KERNEL   $(DEFINES) -o "$@" -c "$<"


OBJECTS_Vision2014_partialImage = Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/FlyingToasters2014.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ADXL345_I2C.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ADXL345_SPI.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Accelerometer.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogChannel.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogModule.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogPotentiometer.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogTrigger.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogTriggerOutput.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/AnalogIOButton.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/Button.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ButtonScheduler.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/CancelButtonScheduler.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/DigitalIOButton.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/HeldButtonScheduler.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/InternalButton.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/JoystickButton.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/NetworkButton.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/PressedButtonScheduler.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ReleasedButtonScheduler.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ToggleButtonScheduler.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/Trigger.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/CANJaguar.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Command.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/CommandGroup.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/CommandGroupEntry.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PIDCommand.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PIDSubsystem.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PrintCommand.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Scheduler.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/StartCommand.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Subsystem.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitCommand.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitForChildren.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitUntilCommand.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Compressor.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Counter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Dashboard.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalInput.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalModule.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalOutput.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalSource.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DoubleSolenoid.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStation.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStationEnhancedIO.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStationLCD.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Encoder.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Error.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ErrorBase.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/GearTooth.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Gyro.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/HiTechnicColorSensor.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/HiTechnicCompass.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/I2C.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/InterruptableSensorBase.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/IterativeRobot.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Jaguar.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Joystick.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Kinect.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/KinectStick.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/LiveWindow/LiveWindow.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/LiveWindow/LiveWindowStatusListener.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Module.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/MotorSafetyHelper.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Notifier.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/OSAL/Synchronized.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/OSAL/Task.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/PIDController.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/PWM.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Preferences.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Relay.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Resource.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/RobotBase.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/RobotDrive.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SPI.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SafePWM.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SensorBase.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SerialPort.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Servo.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SimpleRobot.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SmartDashboard/SendableChooser.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SmartDashboard/SmartDashboard.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Solenoid.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SolenoidBase.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Synchronized.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Talon.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Task.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Timer.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Ultrasonic.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Utility.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Victor.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/AxisCamera.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/AxisCameraParams.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/BinaryImage.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/ColorImage.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/EnumCameraParameter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/HSLImage.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/ImageBase.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/IntCameraParameter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/MonoImage.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/PCVideoServer.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/RGBImage.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/Threshold.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/AxisCamera.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/BaeUtilities.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/FrcError.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/TrackAPI.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/VisionAPI.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Watchdog.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTable.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableConnectionListenerAdapter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableKeyListenerAdapter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableListenerAdapter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableMode.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableProvider.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableSubListenerAdapter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/AbstractNetworkTableEntryStore.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/NetworkTableEntry.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/NetworkTableNode.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/OutgoingEntryReciever.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/TableKeyExistsWithDifferentTypeException.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/TransactionDirtier.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/WriteManager.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientConnectionAdapter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientConnectionState.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientNetworkTableEntryStore.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/NetworkTableClient.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/BadMessageException.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/ConnectionMonitorThread.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/DataIOStream.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/NetworkTableConnection.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/NetworkTableServer.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionAdapter.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionList.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionState.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerIncomingStreamMonitor.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerNetworkTableEntryStore.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/FDIOStream.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketServerStreamProvider.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketStreamFactory.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketStreams.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/thread/DefaultThreadManger.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ArrayData.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ArrayEntryType.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/BooleanArray.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ComplexData.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ComplexEntryType.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/DefaultEntryTypes.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NetworkTableEntryType.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NetworkTableEntryTypeManager.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NumberArray.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/StringArray.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/EOFException.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/IOException.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/IllegalStateException.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/StringCache.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/System.o \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/tables/TableKeyNotDefinedException.o

Vision2014_partialImage/$(MODE_DIR)/Vision2014_partialImage.o : $(OBJECTS_Vision2014_partialImage)
	$(TRACE_FLAG)if [ ! -d "`dirname "$@"`" ]; then mkdir -p "`dirname "$@"`"; fi;echo "building $@"; $(TOOL_PATH)ccppc -r -nostdlib -Wl,-X  -o "$@" $(OBJECTS_Vision2014_partialImage) $(LIBPATH) $(LIBS) $(ADDED_LIBPATH) $(ADDED_LIBS)  && if [ "$(EXPAND_DBG)" = "1" ]; then plink "$@";fi

Vision2014_partialImage/$(MODE_DIR)/Vision2014_partialImage_compile_file : $(FILE) ;

_clean :: Vision2014_partialImage/$(MODE_DIR)/Vision2014_partialImage_clean

Vision2014_partialImage/$(MODE_DIR)/Vision2014_partialImage_clean : 
	$(TRACE_FLAG)if [ -d "Vision2014_partialImage" ]; then cd "Vision2014_partialImage"; rm -rf $(MODE_DIR); fi

force : 

DEP_FILES := Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/FlyingToasters2014.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ADXL345_I2C.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ADXL345_SPI.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Accelerometer.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogChannel.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogModule.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogPotentiometer.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogTrigger.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/AnalogTriggerOutput.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/AnalogIOButton.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/Button.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ButtonScheduler.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/CancelButtonScheduler.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/DigitalIOButton.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/HeldButtonScheduler.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/InternalButton.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/JoystickButton.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/NetworkButton.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/PressedButtonScheduler.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ReleasedButtonScheduler.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/ToggleButtonScheduler.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Buttons/Trigger.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/CANJaguar.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Command.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/CommandGroup.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/CommandGroupEntry.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PIDCommand.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PIDSubsystem.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/PrintCommand.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Scheduler.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/StartCommand.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/Subsystem.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitCommand.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitForChildren.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Commands/WaitUntilCommand.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Compressor.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Counter.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Dashboard.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalInput.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalModule.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalOutput.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DigitalSource.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DoubleSolenoid.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStation.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStationEnhancedIO.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/DriverStationLCD.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Encoder.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Error.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/ErrorBase.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/GearTooth.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Gyro.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/HiTechnicColorSensor.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/HiTechnicCompass.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/I2C.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/InterruptableSensorBase.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/IterativeRobot.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Jaguar.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Joystick.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Kinect.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/KinectStick.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/LiveWindow/LiveWindow.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/LiveWindow/LiveWindowStatusListener.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Module.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/MotorSafetyHelper.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Notifier.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/OSAL/Synchronized.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/OSAL/Task.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/PIDController.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/PWM.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Preferences.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Relay.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Resource.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/RobotBase.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/RobotDrive.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SPI.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SafePWM.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SensorBase.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SerialPort.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Servo.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SimpleRobot.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SmartDashboard/SendableChooser.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SmartDashboard/SmartDashboard.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Solenoid.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/SolenoidBase.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Synchronized.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Talon.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Task.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Timer.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Ultrasonic.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Utility.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Victor.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/AxisCamera.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/AxisCameraParams.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/BinaryImage.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/ColorImage.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/EnumCameraParameter.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/HSLImage.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/ImageBase.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/IntCameraParameter.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/MonoImage.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/PCVideoServer.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/RGBImage.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision/Threshold.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/AxisCamera.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/BaeUtilities.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/FrcError.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/TrackAPI.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Vision2009/VisionAPI.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/Watchdog.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTable.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableConnectionListenerAdapter.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableKeyListenerAdapter.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableListenerAdapter.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableMode.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableProvider.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables/NetworkTableSubListenerAdapter.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/AbstractNetworkTableEntryStore.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/NetworkTableEntry.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/NetworkTableNode.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/OutgoingEntryReciever.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/TableKeyExistsWithDifferentTypeException.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/TransactionDirtier.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/WriteManager.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientConnectionAdapter.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientConnectionState.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/ClientNetworkTableEntryStore.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/client/NetworkTableClient.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/BadMessageException.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/ConnectionMonitorThread.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/DataIOStream.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/connection/NetworkTableConnection.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/NetworkTableServer.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionAdapter.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionList.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerConnectionState.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerIncomingStreamMonitor.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/server/ServerNetworkTableEntryStore.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/FDIOStream.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketServerStreamProvider.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketStreamFactory.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/stream/SocketStreams.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/thread/DefaultThreadManger.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ArrayData.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ArrayEntryType.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/BooleanArray.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ComplexData.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/ComplexEntryType.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/DefaultEntryTypes.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NetworkTableEntryType.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NetworkTableEntryTypeManager.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/NumberArray.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/type/StringArray.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/EOFException.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/IOException.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/IllegalStateException.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/StringCache.d \
	 Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/networktables2/util/System.d Vision2014_partialImage/$(MODE_DIR)/Objects/FlyingToasters2014/WPILib/tables/TableKeyNotDefinedException.d
-include $(DEP_FILES)



-include $(PRJ_ROOT_DIR)/*.makefile

-include *.makefile

main_all : external_build $(PROJECT_TARGETS)
	@echo "make: built targets of `pwd`"

# entry point for extending the build
external_build ::
	@echo ""

# main entry point for pre processing prior to the build
pre_build :: $(PRE_BUILD_STEP) generate_sources
	@echo ""

# entry point for generating sources prior to the build
generate_sources ::
	@echo ""

# main entry point for post processing after the build
post_build :: $(POST_BUILD_STEP) deploy_output
	@echo ""

# entry point for deploying output after the build
deploy_output ::
	@echo ""

clean :: external_clean $(CLEAN_STEP) _clean

# entry point for extending the build clean
external_clean ::
	@echo ""
