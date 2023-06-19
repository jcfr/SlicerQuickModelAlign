#-----------------------------------------------------------------------------
set(MODULE_NAME QuickModelAlign)

#-----------------------------------------------------------------------------
set(MODULE_PYTHON_SCRIPTS
  ${MODULE_NAME}.py
  )

set(MODULE_PYTHON_RESOURCES
  Resources/Icons/${MODULE_NAME}.png
  Resources/CustomColorMaps/red.txt
  Resources/CustomColorMaps/blue.txt
  )

#-----------------------------------------------------------------------------
slicerMacroBuildScriptedModule(
  NAME ${MODULE_NAME}
  SCRIPTS ${MODULE_PYTHON_SCRIPTS}
  RESOURCES ${MODULE_PYTHON_RESOURCES}
  WITH_GENERIC_TESTS
  )


project(QuickModelAlign)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/seanchoi0519/SlicerQuickModelAlign")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Sean Choi")
set(EXTENSION_DESCRIPTION "Testing Align software")
set(EXTENSION_ICONURL "https://github.com/seanchoi0519/SlicerQuickModelAlign/blob/main/QuickModelAlign.png")
set(EXTENSION_SCREENSHOTURLS "https://github.com/seanchoi0519/SlicerQuickModelAlign/blob/main/QuickModelAlign.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(QuickModelAlign)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})

