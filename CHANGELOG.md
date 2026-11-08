# Changelog

All notable changes to `skuul` will be documented in this file.

## [3.1.3](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/compare/v3.1.2...v3.1.3) (2026-11-08)


### Bug Fixes

* make documentation accessible from the app ([#443](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/issues/443)) ([63db1de](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/commit/63db1ded6c753e8cd04f71cf7416d327a05d37a5))


### Miscellaneous Chores

* **main:** release 3.1.1 ([#440](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/issues/440)) ([c1309a0](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/commit/c1309a01b9d3d21073d962b3f25506d5b12d931e))
* **main:** release 3.1.1 ([#442](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/issues/442)) ([795aabe](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/commit/795aabe3c8a01ce330a2699ee55d90d4af79d748))
* **main:** release 3.1.2 ([#444](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/issues/444)) ([ad37363](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/commit/ad3736307b338ee2b0c3a06086444cb55239c57b))
* set up Release Please and a security policy ([#439](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/issues/439)) ([358e0e8](https://github.com/Turkiye-Acik-Kaynak-Yazilim-Grubu/skuul/commit/358e0e8266e3d06fccdbb8b52a67b9c064959f95))

## [3.1.2](https://github.com/yungifez/skuul/compare/v3.1.1...v3.1.2) (2026-10-28)


### Bug Fixes

* make documentation accessible from the app ([#443](https://github.com/yungifez/skuul/issues/443)) ([63db1de](https://github.com/yungifez/skuul/commit/63db1ded6c753e8cd04f71cf7416d327a05d37a5))


### Miscellaneous Chores

* **main:** release 3.1.1 ([#442](https://github.com/yungifez/skuul/issues/442)) ([795aabe](https://github.com/yungifez/skuul/commit/795aabe3c8a01ce330a2699ee55d90d4af79d748))

## [3.1.1](https://github.com/yungifez/skuul/compare/v3.1.0...v3.1.1) (2026-10-24)


### Miscellaneous Chores

* set up Release Please and a security policy ([#439](https://github.com/yungifez/skuul/issues/439)) ([358e0e8](https://github.com/yungifez/skuul/commit/358e0e8266e3d06fccdbb8b52a67b9c064959f95))

## [3.1.0](https://github.com/yungifez/skuul/compare/v3.0.2...v3.1.0) (2026-10-24)

Skuul now supports both ways of teaching: learners who stay in one class all day, and learners who move between subjects.

### Features

* A level group, such as "Upper school", can name learners from all its levels.
* Subject setup starts from the roster mode of the campus's teaching model. A subject with named learners checks its capacity.
* A subject can have its own timetable and its own name, such as "Algebra B · Mathematics".
* Learners and teachers see a personal week that combines every timetable that applies to them.
* The timetable clash check warns when learners of two subjects are placed at the same time.
* Each subject has a lesson register. It lists the learners on the subject's roster, from any section. Only a current teacher of the subject can take it.
* A notice can go to the learners of chosen subjects.
* Rankings can compare the learners of one subject with named learners, by their result in that subject.
* A campus with no daily register counts lesson registers on the dashboard and in the portal.

### Bug Fixes

* The portal timetable stays on the learner's own campus.
* Roll-forward copies each subject with named learners once.
* A teacher of one section of a class can record syllabus coverage for that class.
* On a whole-level subject, a teacher of some sections sees and marks only their own learners in the gradebook.
* Update Livewire to 4.4.8 and Vite to 6.4.5 for security advisories.

### Upgrade notes

This release has two migrations. They add subject timetables and lesson registers. Back up the database, then update with `php artisan skuul:update` or check out the `v3.1.0` tag.

## Earlier releases

See the [GitHub releases](https://github.com/yungifez/skuul/releases) for v3.0.2 and older.
