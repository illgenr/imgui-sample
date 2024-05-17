# select the 3D backend for sokol_gfx.h and sokol_app.h
add_definitions(-D${sokol_backend})

fips_ide_group(Samples)
fips_begin_app(imgui-sample windowed)
    fips_files(imgui-sapp.cc)
    # use sokol-cpp for testing here, this isn't required though
    fips_deps(sokol-cpp imgui)
    if (FIPS_IOS)
        fips_files(ios-info.plist)
    endif()
fips_end_app()

