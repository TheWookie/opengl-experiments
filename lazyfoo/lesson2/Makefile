#OBJS specifies which files to compile as part of the project
OBJS = LUtil.cpp main.cpp
#CC specifies which compiler we're using
CC = g++
#COMPILER_FLAGS specifies the additional compilation options we're using
# -w suppresses all warnings
COMPILER_FLAGS = -w
#LINKER_FLAGS specifies the libraries we're linking against
LINKER_FLAGS = -lGL -lGLU -lglut
#Output directory
TARGETDIR = ./bin
#OBJ_NAME specifies the name of our exectuable
OBJ_NAME = $(TARGETDIR)/application.bin

#This is the target that compiles our executable
all : $(OBJS)
	@mkdir -p $(TARGETDIR)
	$(CC) $(OBJS) $(COMPILER_FLAGS) $(LINKER_FLAGS) -o $(OBJ_NAME)

clean:
	find -type f -name "*.gch" -exec rm {} \;
	rm -rf $(TARGETDIR)
