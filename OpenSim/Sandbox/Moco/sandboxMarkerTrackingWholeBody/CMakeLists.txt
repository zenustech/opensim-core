MocoAddSandboxExecutable(NAME sandboxMarkerTrackingWholeBody
        LIB_DEPENDS osimMoco tropter
        SOURCE_FILES
            MuscleLikeCoordinateActuator.cpp
            MuscleLikeCoordinateActuator.h
        )

# Copy example model and data files to use in Sandbox.
file(COPY "${PROJECT_SOURCE_DIR}/Bindings/Java/Matlab/examples/Moco/exampleMarkerTracking10DOF/marker_trajectories.trc"
    "${PROJECT_SOURCE_DIR}/Bindings/Java/Matlab/examples/Moco/exampleMarkerTracking10DOF/subject01.osim"
    "${PROJECT_SOURCE_DIR}/Bindings/Java/Matlab/examples/Moco/exampleMarkerTracking10DOF/state_reference.mot"
        DESTINATION "${CMAKE_CURRENT_BINARY_DIR}")
