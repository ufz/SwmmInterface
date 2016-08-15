add_library ( SWMM
    SWMM/src/climate.c
    SWMM/src/controls.c
    SWMM/src/culvert.c
    SWMM/src/datetime.c
    SWMM/src/dwflow.c
    SWMM/src/dynwave.c
    SWMM/src/error.c
    SWMM/src/exfil.c
    SWMM/src/findroot.c
    SWMM/src/flowrout.c
    SWMM/src/forcmain.c
    SWMM/src/gage.c
    SWMM/src/gwater.c
    SWMM/src/hash.c
    SWMM/src/hotstart.c
    SWMM/src/iface.c
    SWMM/src/infil.c
    SWMM/src/inflow.c
    SWMM/src/input.c
    SWMM/src/inputrpt.c
    SWMM/src/keywords.c
    SWMM/src/kinwave.c
    SWMM/src/landuse.c
    SWMM/src/lid.c
    SWMM/src/lidproc.c
    SWMM/src/link.c
    SWMM/src/massbal.c
    SWMM/src/mathexpr.c
    SWMM/src/mempool.c
    SWMM/src/node.c
    SWMM/src/odesolve.c
    SWMM/src/output.c
    SWMM/src/project.c
    SWMM/src/qualrout.c
    SWMM/src/rain.c
    SWMM/src/rdii.c
    SWMM/src/report.c
    SWMM/src/roadway.c
    SWMM/src/routing.c
    SWMM/src/runoff.c
    SWMM/src/shape.c
    SWMM/src/snow.c
    SWMM/src/stats.c
    SWMM/src/statsrpt.c
    SWMM/src/subcatch.c
    SWMM/src/surfqual.c
    SWMM/src/swmm5.c
    SWMM/src/table.c
    SWMM/src/toposort.c
    SWMM/src/transect.c
    SWMM/src/treatmnt.c
    SWMM/src/xsect.c
)

add_library ( SwmmInterface
    swmm5_iface.h
    swmm5_iface.c
)

target_link_libraries (SwmmInterface SWMM)

include_directories ( SWMM/src )
