---
layout: release_note_release
title: "StoRM v.1.11.1 - release notes"
release_date: "03.06.2013"
release_description: "This was the first update for StoRM in EMI-3."
release_title: "StoRM v.1.11.1"
release_rfcs:
    - id: STOR-172
      type: bug
      title: StoRM now correctly publishes information about storage area sizes in the information system.
    - id: STOR-148
      type: bug
      title: StoRM now leverages quota limits information gathered from the underlying GPFS filesystem to compute a storage area size
    - id: STOR-10
      type: bug
      title: StoRM now gets quota information directly from GPFS filesystem
    - id: STOR-130
      type: bug
      title: StoRM GridHTTPs server is now correctly registered to start at system boot.
    - id: STOR-117
      type: bug
      title: Duplicate prepare-to-get calls on a SURL are now correctly handled
    - id: STOR-113
      type: bug
      title: The StoRM YAIM module does not try to configure permissions on existing configured storage areas. It is assumed (and documented) that the correct permissions are set by the system administrator before running YAIM.
    - id: STOR-109
      type: bug
      title: The Java JDK dependency has been fixed so that all StoRM packages explicitly requires OpenJDK.
    - id: STOR-230
      type: feature
      title: The StoRM WebDAV PROPFIND implementation performance has been improved.
release_components:
    - name: StoRM Backend
      package: storm-backend-server
      version: 1.11.1
    - name: StoRM native libs
      package: storm-native-libs
      version: 1.0.1
    - name: StoRM GridHTTPs
      package: storm-gridhttps-server
      version: 2.0.1
    - name: YAIM StoRM
      package: yaim-storm
      version: 4.3.2
    - name: StoRM dynamic info
      package: storm-dynamic-info-provider
      version: 1.7.6
---