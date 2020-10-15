==changelog for openebs/libcstor ===
- [libcstor]  Adding changelog for v2.1.0 (1874b18) (@mynktl)


==changelog for openebs/cstor ===
- [cstor]  Adding changelog for v2.1.0 (da69f4f) (@mynktl)


==changelog for openebs/istgt ===
- [istgt]  chore(doc): add 2.1.0 changelog in the repo (042fcf5) (@mittachaitu)


==changelog for openebs/velero-plugin ===
- [velero-plugin]  Adding changelog for v2.1.0 (063e9c5) (@mynktl)
- [velero-plugin]  chore(travis): add recipients for travis notifications. (fcd1dca) (@sonasingh46)
- [velero-plugin]  feat(log): making log level available for velero plugin (#116) (9a77ff7) (@pawanpraka1)
- [velero-plugin]  feat(s3): support to use custom certificate for s3 object storage (#115) (1f816bb) (@mynktl)
- [velero-plugin]  feat(velero): wait for plugin server to be UP before doing backup/restore (#117) (9a3232a) (@pawanpraka1)
- [velero-plugin]  feat(zfspv): adding support to do incremental backup/restore (#121) (5f05863) (@pawanpraka1)
- [velero-plugin]  feat(zfspv): adding support to restore on different setup/nodes (b4ac369) (@pawanpraka1)
- [velero-plugin]  feat(zfspv): use schedule name to identify the scheduled backup (#124) (a4fe177) (@pawanpraka1)
- [velero-plugin]  fix(zfspv): fixing the backup deletion (#129) (ec4d713) (@pawanpraka1)


==changelog for openebs/cstor-csi ===
- [cstor-csi]  chore(changelog): add changelog for 2.1.0 (#121) (d7bf82f) (@sonasingh46)
- [cstor-csi]  chore(travis): add recipients for travis notifications. (#126) (6a32884) (@sonasingh46)
- [cstor-csi]  feat(metrics): add volumes metrics support for raw block volume (b82d383) (@prateekpandey14)
- [cstor-csi]  fix(remount): resolve race condition in remount code (#122) (803448c) (@payes)


==changelog for openebs/cstor-operators ===
- [cstor-operators]  chore(changelog) : add changelog for 2.1.0 (0b31184) (@sonasingh46)
- [cstor-operators]  chore(docs): add csi cstor volume metrics exposed by prometheus (63eebd7) (@prateekpandey14)
- [cstor-operators]  chore(travis): add recipients for travis notifications. (#190) (66475dc) (@sonasingh46)
- [cstor-operators]  chore(version): add 2.2.0 to upgrade matrix (#188) (f97ec6a) (@shubham14bajpai)
- [cstor-operators]  docs(bd-tag): add tutorial for using BD tag feature. (#181) (5abd4c1) (@sonasingh46)
- [cstor-operators]  feat(backup & restore): add v1 support for backup and restore (#182) (1f266bd) (@mittachaitu)
- [cstor-operators]  feat(backup, restore): promote backup and restore controller to use v1 apis (#183) (96760c3) (@mittachaitu)
- [cstor-operators]  feat(CSPC, nodeName changes): add suport to move the CStorPoolInstances to specified node (#167) (5e2f739) (@mittachaitu)
- [cstor-operators]  fix(backup, restore): create backup and restore in cstor.openebs.io/v1 group (#192) (25dd38a) (@mittachaitu)
- [cstor-operators]  fix(restore): use relative labels to fetch CSPI name (#191) (9f7f39e) (@mittachaitu)
- [cstor-operators]  fix(typo): fixes typo in cstor operator log messages (#186) (b1be5f9) (@nsathyaseelan)
- [cstor-operators]  fix various language issues on homepage (#176) (3c54921) (@Didier Durand)
- [cstor-operators]  refact(crds): update crds based on new api spec changes (#189) (c3a347e) (@prateekpandey14)


==changelog for openebs/api ===
- [api]   feat(backup & restore): add v1 apis of cStor backup and restore (#58) (b9ef3e7) (@mittachaitu)
- [api]  feat(changelog): add changelog for 2.1.0 (1725eac) (@sonasingh46)
- [api]  refact(crds): update API spec type description based on new changes (#71) (3ab926b) (@prateekpandey14)


==changelog for openebs/jiva ===
- [jiva]  chore(license): add license-check for .go , .sh , Dockerfile and Makefile (#328) (96e6c30) (@payes)
- [jiva]  update(README): add HackMD badge (#327) (73dfc13) (@payes)


==changelog for openebs/maya ===
- [maya]  chore(CHANGELOG): add changelogs for v2.1.0 (#1753) (c51d91e) (@shubham14bajpai)
- [maya]  chore(version): add 2.2.0 to upgrade matrix (#1758) (fe2824a) (@shubham14bajpai)


==changelog for openebs/external-storage ===


==changelog for openebs/upgrade ===
- [upgrade]  Added all badges (712aca9) (@Debojyoti Chakraborty)
- [upgrade]  Added all the badges in upgrade (#55) (52d7173) (@shubham14bajpai)
- [upgrade]  chore : Added pull request and Issue template (#54) (3640a16) (@Siddharth Mishra)
- [upgrade]  chore(CHANGELOG): add changelogs for v2.1.0 (#51) (1e1e518) (@shubham14bajpai)
- [upgrade]   chore(travis): add recipients for travis notifications. (#60) (22179cc) (@sonasingh46)
- [upgrade]  feat(cstor): add support for backup/restore upgrade & migration (#59) (ff71d09) (@shubham14bajpai)
- [upgrade]  feat(migrate): add support to correct blockdevices in spc before migration (#53) (7c12aed) (@shubham14bajpai)
- [upgrade]  fix(travis): update migrate jobs to use correct imageorg images (#61) (59e377f) (@shubham14bajpai)
- [upgrade]  refact(migration): update volume migration to run in parallel (#52) (2eb9a3d) (@shubham14bajpai)
- [upgrade]  Replace reflect.DeepEqual() with "github.com/google/go-cmp/cmp" (#58) (b2d33c8) (@Aswin Gopinathan)
- [upgrade]  Update README.md (82f3688) (@Debojyoti Chakraborty)
- [upgrade]  Update the main README with info and link upgrade & migration docs #3145 (#57) (6c3115d) (@Naveenkhasyap)


==changelog for openebs/linux-utils ===
- [linux-utils]  chore(build): tag libcstor as a downstream repo (ef4802a) (@mittachaitu)


==changelog for openebs/node-disk-manager ===
- [node-disk-manager]  feat(metrics): exporting seachest data to prometheus (#461) (0baecdc) (@harshthakur9030)
- [node-disk-manager]  feat(Name): Add Name as a meta info for partitions created by OpenEBS (#494) (6c2ff64) (@Aditya Vats)
- [node-disk-manager]  fix(disk-filter): Exclude multiple os disk paths (#481) (f93d0fd) (@rahulchheda)
- [node-disk-manager]  fix(mount): detect real device when using /dev/root (#492) (6f12166) (@zlymeda)
- [node-disk-manager]  fix(partition): check if filesystem exists on disk before creating partitions (8232952) (@akhilerm)
- [node-disk-manager]  fix(sysfs,udev): add additional verbose logs in udev probe (3e81357) (@akhilerm)
- [node-disk-manager]  refact(sysfs): add a generic sysfs package for handling sysfs on the host (#489) (d4caf92) (@akhilerm)
- [node-disk-manager]  Updating changelog for v0.8.1 (287edbe) (@akhilerm)
- [node-disk-manager]  Updating changelog for v0.8.1-RC1 (a4f5391) (@akhilerm)


==changelog for openebs/zfs-localpv ===
- [zfs-localpv]  add go report card badge for ZFS-LocalPV (#223) (baa00bf) (@Naveenkhasyap)
- [zfs-localpv]  chore(changelog): adding change log for v1.0.0 release (d4385bd) (@pawanpraka1)
- [zfs-localpv]  chore(doc): adding docs for backup and restore (c2e4fae) (@pawanpraka1)
- [zfs-localpv]  chore(doc): updating the doc with supported storageclass parameters (#212) (8298644) (@pawanpraka1)
- [zfs-localpv]  chore(yaml): removing centos yamls from the repo (ed0e078) (@pawanpraka1)
- [zfs-localpv]  chore(yaml): updating v1.0.x branch with the 1.0.0 image tag (06f67eb) (@pawanpraka1)
- [zfs-localpv]  feat(backup,restore): adding validation for backup and restore (ede8422) (@pawanpraka1)


==changelog for openebs/e2e-tests ===
- [e2e-tests]  Create LICENSE.txt (#534) (100d9a0) (@harikrishnajiju)
- [e2e-tests]  feat: add missing copyright message in test-mem.py #535 (#537) (0daca3b) (@Saloni Goyal)
- [e2e-tests]  feat(exp): backup & restore e2e-test for zfs-localpv (#538) (ccd5ea6) (@w3aman)
- [e2e-tests]  feat[migration]: Automated the test case to migrate spc pool and cstor volumes (#530) (eb6a39b) (@nsathyaseelan)
- [e2e-tests]  Modified the cstor operator provisione test case to obtain the operator files from charts (#529) (5bf94ef) (@nsathyaseelan)
- [e2e-tests]  refact(doc)update readme (#531) (46e651c) (@gprasath)
- [e2e-tests]  refactor[cstor-operator]: Modified the cstor operator provision test script (#541) (f213943) (@nsathyaseelan)
- [e2e-tests]  refactor[migration]: Modified the application scaledown and scaleup util for volume migration test (#542) (9ceb0a8) (@nsathyaseelan)
- [e2e-tests]  refactor[migration]: Modified the application scaledown and scaleup util for volume migration test (#543) (c12974c) (@nsathyaseelan)
- [e2e-tests]  refactor(migration): Updated the application scaledown tasks for pool migration test (#544) (583a759) (@nsathyaseelan)
- [e2e-tests]  refactor(pool-delete): Modified the task to check the cvr status before deleting the pool (#539) (090ca4f) (@nsathyaseelan)
- [e2e-tests]  refactor(script): Add retry in snapshot verify task in cstor csi snapshot test (#528) (4733c99) (@shashank855)
- [e2e-tests]  refact(rothreshold): increase the iteration count while fetching readonly status of csp (#527) (fb12140) (@gprasath)
- [e2e-tests]  Update README.md (07cfd7c) (@gprasath)
- [e2e-tests]  Update test_health.py (21f6153) (@Aman Singh)
- [e2e-tests]  update test-mem (#540) (cd5c014) (@gprasath)


==changelog for openebs/openebs-docs ===
- [openebs-docs]  chore(release): update references to 2.1.0 (294983d) (@kmova)
- [openebs-docs]  chore(release): update references to 2.1.0 in cstor (dd9a952) (@kmova)
- [openebs-docs]  fix(uninstall): verify bds are removed (#872) (845354b) (@kmova)


==changelog for openebs/openebs ===
- [openebs]  [#3203] Translate documentation to Brazilian Portuguese (#3205) (1335d7c) (@Lucas Queiroz)
- [openebs]  Adding Multiarch Setup to Adopters.md (#3215) (7d085dc) (@Daniel Sand)
- [openebs]  add section for helping with contributions (d69d4bd) (@kmova)
- [openebs]  chore(docs): fix typo in oep-template.md (#3243) (e9e95f6) (@Vishal Kichloo)
- [openebs]  chore(docs): fix typos in Roadmap.md file (#3232) (183f2c3) (@Karan Singh Bisht)
- [openebs]  chore(docs): incorporate comments on text (881bc43) (@kmova)
- [openebs]  chore(docs): update source repository details (f850c03) (@kmova)
- [openebs]  chore(docs):Update URLs and dead link (#3154) (9dca8cc) (@sabbatum)
- [openebs]  chore(doc): update the order of release tagging (a3c1706) (@mittachaitu)
- [openebs]  chore(roadmap): incorporate review comments on dashboard (e686591) (@kmova)
- [openebs]  chore(roadmap): rename features to backlogs (f7344bf) (@kmova)
- [openebs]  chore(upgrade): update upgrade README with 2.1.0 steps (b2013b7) (@shubham14bajpai)
- [openebs]  Delete cassandra-loadgen.yaml (c34fc4c) (@ranjithwingrider)
- [openebs]  Delete cassandra-service.yaml (f264cf3) (@ranjithwingrider)
- [openebs]  Delete cassandra-statefulset.yaml (6bbe76d) (@ranjithwingrider)
- [openebs]  DOCS: Add Gujarati language translations (#3172) (aad634a) (@Aryan Rawlani)
- [openebs]  docs(adopters): add hamravesh and tobg services to adopters (#3129) (b162fca) (@akhilerm)
- [openebs]  docs(roadmap): update information in roadmap.md (3d0a5ec) (@kmova)
- [openebs]  docs(roadmap): update Mayastor related backlogs (68ce5b4) (@kmova)
- [openebs]  docs(roadmap): update NDM and cStor backlogs (58203df) (@kmova)
- [openebs]  feat(readme): add README.md & CONTRITUBING.md in French (4f95662) (@André Aubin)
- [openebs]  fix(YAML): Update MinIO according to latest API (#3130) (aa2df01) (@ranjithwingrider)
- [openebs]  incorporate text review comments (926dce4) (@kmova)
- [openebs]  Merge pull request #3138 from kmova/update-repo-info (16009f9) (@muratkars)
- [openebs]  Merge pull request #3141 from kmova/update-roadmap-post-2.0 (dbd37a9) (@muratkars)
- [openebs]  Merge pull request #3153 from ranjithwingrider/cassandra-ranjith (51277b7) (@muratkars)
- [openebs]  oep(cstor): proposal to migrate pools and volumes from old schema to new schema (#2840) (5e4462f) (@shubham14bajpai)
- [openebs]  oep(ndm): proposal for unique disk identification (#2666) (f221659) (@akhilerm)
- [openebs]  OEP(pool migration): add support for CStor pools migration when underlying disks are migrated to another node (#3113) (5d073d3) (@mittachaitu)
- [openebs]  Update LICENSE (#3156) (2eab955) (@Julian)
- [openebs]  Update README.md (b25455c) (@ranjithwingrider)
- [openebs]  Update README.md (e8411a5) (@ranjithwingrider)


==changelog for openebs/monitor-pv ===




==changelog for openebs/rawfile-localpv ===


==changelog for openebs/charts ===
- [charts]  [stable/openebs]:  update NDM version to 0.8.2 (c0e240f) (@akhilerm)
- [charts]  [stable/openebs]: update openebs charts to 2.0.0 release (bb67af5) (@mittachaitu)


==changelog for openebs/charts ===
- [charts]  chore(operator): update ndm version to 0.8.2 (6b28893) (@akhilerm)
- [charts]  chore(operator, yaml): add openebs operator 2.1.0 (#146) (1207d37) (@akhilerm)
- [charts]  chore(release): add script to check for images (edd9f98) (@akhilerm)
- [charts]  chore(release): update release scripts to 2.2.0 tags (939a64d) (@kmova)
- [charts]  chore(release): update release scripts with 2.1.0 (33a23b6) (@kmova)
- [charts]  chore(release): update to 2.2.0-RC1 tag (1f1ec6b) (@kmova)
- [charts]  chore(YAML): Create openebs-operator-2.1.0-aws.yaml (170b139) (@ranjithwingrider)
- [charts]  chore(YAML): Update openebs-operator-2.1.0-aws.yaml (07654d7) (@ranjithwingrider)
- [charts]  fix(cstor-operator): add ephemeral support in CSIDriver VolumeLifecycleModes (#150) (c3351b3) (@mittachaitu)
- [charts]  Merge branch 'gh-pages' of https://github.com/openebs/charts into gh-pages (63564de) (@kmova)
- [charts]  Merge pull request #148 from ranjithwingrider/gh-pages (71ac51a) (@muratkars)
- [charts]  refact(cstor-operator): add missing upgradetasks CRD (#152) (2c51f8a) (@prateekpandey14)
- [charts]  Update index.yaml (523a679) (@kmova)
- [charts]  Update index.yaml (aabb9f5) (@kmova)


==changelog for openebs/website ===
- [website]  Add notification banner of hacktoberfest (#54) (e920090) (@IsAmrish)
- [website]  Fix typos in community page (#53) (394d926) (@IsAmrish)
- [website]  Update community page and remove community-meet page (#52) (f07fea4) (@IsAmrish)


==changelog for openebs/performance-benchmark ===


