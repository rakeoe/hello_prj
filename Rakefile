# -*- ruby -*-

#
# RakeOE Project Rakefile
#
# RakeOE is sensitive to the following environment variables:
#
# RELEASE         If set, compilation will be done with RELEASE settings
#                 (Optimization level, no debugging symbols). The symbol -DRELEASE
#                 is passed to the compiler via CFLAGS/CXXFLAGS
#
# SW_VERSION_ENV  Software version string. This string will be passed via CFLAGS/CXXFLAGS as
#                 -DPROGRAM_VERSION
#
# TOOLCHAIN_ENV   Open Embedded compatible toolchain definition file. 
# 
#
require 'rubygems'
require 'rakeoe'

# Override some defaults
config = RakeOE::Config.new

# Assign application and library source directories and the build directory
config.directories = {
          :apps =>         %w[src],
          :libs =>         [],
          :build =>        'build',
          :deploy =>       'deploy'
        }

# Do stuff
tool = RakeOE::init(config)

# EOF
