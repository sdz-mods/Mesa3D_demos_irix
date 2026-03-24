# Mesa3D 3.5.0 demos

Mesa3D 3.5.0 demos for IRIX.


## Building

### Prerequisites

Install the complete IRIX development environment:

- MIPSPro 7.4.4 compiler (install 7.4, then patch to 7.4.4m)
- Development Foundation 1.3
- Development Libraries February 2002 (latest version)

Build and install the IRIX 3dfx kernel driver:
- https://github.com/sdz-mods/tdfx_irix

Build and install the glide2x IRIX port:
- https://github.com/sdz-mods/glide_irix

Build and install the MesaFX glide2x Irix port:
- https://github.com/sdz-mods/MesaFX_irix


### Build and Install

```csh
#clone or copy this repo onto the target system, e.g. /usr/3dfx_irix/Mesa32_demos_irix
cd /usr/3dfx_irix/Mesa32_demos_irix
smake -f Makefile.irixfx MESA_ROOT=/usr/3dfx_irix/MesaFX_irix

#output binaries are copied to the bin directory
#not all demos are built
ls /usr/3dfx_irix/Mesa3D_demos_irix/bin/
bounce*         gears*          geartrain*      geartrain.dat*  glinfo*         gltestperf*     glutfx*         isosurf.dat*    morph3d*        paltex*         ray*            renormal*       spectex*        terrain*        terrain.dat*    texenv*         texobj*         trispd*
```


## Tested with

- IP32, RM7000C CPU, Irix 6.5.30, Voodoo1, tdfx_irix, glide_irix, MesaFX_irix


## License

Source code is licensed under the MIT License.
