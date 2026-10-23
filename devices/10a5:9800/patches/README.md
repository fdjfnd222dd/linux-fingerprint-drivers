# Patches for FPC fpcmoh (10a5:9800)

- `0001-fpcmoh-support-10a5-9800-v1.94.10.patch` - libfprint MR !396 rebased
  onto libfprint tag **v1.94.10**, base commit
  `0c97a47d8ef405cd577b87058c1e89cae9d242e7`
  (`git apply --check` passes on a clean checkout). On top of the MR it resolves
  conflicts with the realtek and focaltech_moc drivers, drops 10a5:9800 from
  the unsupported-devices list, and adds a `fpcbep_dir` meson option to locate
  the proprietary `libfpcbep.so`. Build steps are in `../README.md`.

For other libfprint versions the driver is distributed via the
`libfprint-fpcmoh-git` AUR package (see `../CREDITS`). Remember the device also
needs the accompanying udev rules.
