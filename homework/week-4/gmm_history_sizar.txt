 1471  cd gitstery/
 1472  clear
 1473  git cat-file blob HEAD:instructions.txt
 1474  echo "John Doe" | git hash-object --stdin | grep -iq -f /dev/stdin <(git show solution) && echo 'You found the murderer!' || echo 'No cigar, chief... Try again.'
 1475  ls -lh
 1476  cd Desktop/Class/gitstery/
 1477  ls
 1478  git log
 1479  git cat-file blob HEAD:instructions.txt
 1480  git checkout gtpd-archive
 1481  git log
 1482  git checkout detectives/kpumbinner
 1483  git log
 1484  git blame access.log | grep BACKDOOR_332
 1485  ls
 1486  cd evidence/
 1487  ls
 1488  git blame access.log | grep BACKDOOR_332
 1489  cd ..
 1490  git cat-file blob HEAD:instructions.txt
 1491  git cat-file blob HEAD:residents.txt
 1492  cat residents.txt | grep "Lyndon"
 1493  cat residents.txt | grep "Cosmo"
 1494  cat residents.txt | grep "Brock Stuickard"
 1495  cd evidence/
 1496  git blame access.log | grep BACKDOOR_332
 1497  cd ..
 1498  git cat-file blob HEAD:instructions.txt
 1499  git tag -l
 1500  git tag -l | grep "tamworth"
 1501  git tag -l | grep "Balcombe"
 1502  git tag -l | grep "balcombe"
 1503  git tag -l | grep "beaconside"
 1504  git checkout street/tamworth_drive
 1505  git cat-file blob HEAD:instructions.txt
 1506  git log
 1507  git log | grep "/73 "
 1508  git log
 1509  git checkout 3c2751bbf3bf577b462237bf5848c25ac0de460d
 1510  git log
 1511  git checkout 908ca6a49d54bbc44dbbfa8195da2206ef8128a5
 1512  git log
 1513  git checkout f8a5b218b1eaee3b111ae5ef536f919e8d3afca2
 1514  ls
 1515  cat investigate
 1516  git cat-file -p 22f733298423b814f1da31bee3e0063c72ed6e71
 1517  git checkout street/balcombe_close
 1518  git log
 1519  git checkout bc6870d8093a33d9a69acc94a1cda16ee2d7195d
 1520  cat investigate
 1521  git cat-file -p c8411c73e49372dbdb644beef2ea841b403fc476%
 1522  git cat-file -p c8411c73e49372dbdb644beef2ea841b403fc476
 1523  git checkout street/beaconside
 1524  git log
 1525  git checkout 92f6e05c6aa06c791f402d7e19649fa1f0ec76c6
 1526  cat investigate
 1527  git cat-file -p d1278ebc164050fe1e5526fbba6a8cfbe763f1d2
 1528  echo "Cosmo Siwkonk" | git hash-object --stdin | grep -iq -f /dev/stdin <(git show solution) && echo 'You found the murderer!' || echo 'No cigar, chief... Try again.'
 1529  history > gmm_history_sizar.md
 1530  cat gmm_history_sizar.md
 1531  rm gmm_history_sizar.md
 1532  history | tail -n 59 > gmm_history_sizar.md
 1533  cat gmm_history_sizar.md
