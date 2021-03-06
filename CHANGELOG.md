# Change Log

## [v0.20180519.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20180519.0) (2018-05-19)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20180429.0...v0.20180519.0)

- Add `"Previous Ubuntu"` to `BuildWorkerImageName` enum.

## [v0.20180429.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20180429.0) (2018-04-29)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20180426.0...v0.20180429.0)

- Add `Deny` group with `DenyAllProjectsEnvironments` permission.

## [v0.20180426.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20180426.0) (2018-04-26)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20171123.0...v0.20180426.0)

- Add `recordsNumber` query param to `getProjectDeployments`.
- Add `OctopusPackage` to `ArtifactType` enum.
- Add `ElasticBeanstalkPackage` to `ArtifactType` enum.
- Add `matrixExcept` to `ProjectConfiguration`.
- Add `matrixOnly` to `ProjectConfiguration`.
- Add `packageDotnetConsoleProjects` to `ProjectConfiguration`.
- Add `packageAspNetCoreProjects` to `ProjectConfiguration`.
- Add `packageWebApplicationProjectsOctopus` to `ProjectConfiguration`.
- Add `packageWebApplicationProjectsBeanstalk` to `ProjectConfiguration`.
- Add `stacks` array to `ProjectConfiguration`.
- Add `rollingBuildsOnlyForPullRequests` to `Project`.
- Add `pwsh` to `ScriptLanguages`.

## [v0.20171123.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20171123.0) (2017-11-23)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20171031.0...v0.20171123.0)

- Add `getBuildArtifacts` operation and `ArtifactModel` schema for response.
- Add `getBuildArtifact` operation.
- Add `getProjectArtifact` operation.
- Add `tags` property to `DeploymentEnvironment`.
- Add `isPrivateProject` property to `NuGetFeed`.
- Add enumeration values to `ArtifactType` based on `Push-AppveyorArtifact`
  cmdlet on build workers.
- Remove `name` property requirement from `Artifact`.

## [v0.20171031.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20171031.0) (2017-10-31)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20171023.0...v0.20171031.0)

- Add `getProjectEnvironmentVariables` operation.
- Add `updateProjectEnvironmentVariables` operation.

## [v0.20171023.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20171023.0) (2017-10-23)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20171021.0...v0.20171023.0)

- Add `dotnetCsprojAssemblyVersionFormat` to `ProjectConfiguration`.
- Add `dotnetCsprojFileVersionFormat` to `ProjectConfiguration`.
- Add `dotnetCsprojInformationalVersionFormat` to `ProjectConfiguration`.

## [v0.20171021.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20171021.0) (2017-10-21)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20171019.0...v0.20171021.0)

- Add `pro-vs2013` to `BuildCloudName`.

## [v0.20171019.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20171019.0) (2017-10-19)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170827.0...v0.20171019.0)

- Add `pro-vs2017` to `BuildCloudName`.

## [v0.20170827.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170827.0) (2017-08-27)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170803.0...v0.20170827.0)

- Add `saveBuildCacheInPullRequests` to `Project`.

## [v0.20170803.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170803.0) (2017-08-03)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170622.0...v0.20170803.0)

- Add `dotnetCsprojFile`, `dotnetCsprojPackageVersionFormat`,
  `dotnetCsprojVersionFormat`, `hotFixScripts` to `ProjectConfiguration`.

## [v0.20170622.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170622.0) (2017-06-22)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170518.0...v0.20170622.0)

- Add `Visual Studio 2017 Preview` to `BuildWorkerImageName`

## [v0.20170518.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170518.0) (2017-05-18)

[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170507.0...v0.20170518.0)
- Add `Ubuntu` to `OSType`, `BuildCloudName`, `BuildWorkerImageName`

## [v0.20170507.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170507.0) (2017-05-07)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170503.0...v0.20170507.0)

- Add `osType` to `BuildJob` and `BuildWorkerImage`.
- Add `rollingBuildsDoNotCancelRunningBuilds` to `Project`.
- Better document `scheduleCrontabExpression`.

## [v0.20170503.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170503.0) (2017-05-03)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170308.0...v0.20170503.0)

- **Breaking**  Rename path parameter for `getProjectStatusBadge` and
  `getProjectBranchStatusBadge` to `statusBadgeId` to match its new source,
  which is the new `statusBadgeId` property of `ProjectWithConfiguration`
  objects.  The value of this property matches `webhookId` (the previous
  parameter source) for existing projects but will differ for new projects.
- Add enumeration values for `BuildCloudName` and `BuildWorkerImageName`.
- Add `matrixExclude` property to `ProjectConfiguration`.
- Additional property documentation strings.
- Bump dependency versions.

## [v0.20170308.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170308.0) (2017-03-08)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170107.1...v0.20170308.0)

- **API Breaking**  `getEnvironments`, `getEnvironmentDeployments`, and
  `getProjectDeployments` responses now include fewer properties.  Introduce
  `*LookupModel` schemas for these abbreviated types (based on the name in the
  XML) and rework the existing schemas to use them where appropriate.
- Add `encryptValue` operation to encrypt a string value for use in
  `StoredValue` properties (e.g. environment variable values).
- Add more documentation for properties with non-obvious behavior.

## [v0.20170107.1](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170107.1) (2017-01-20)
[Full Changelog](https://github.com/kevinoid/appveyor-swagger/compare/v0.20170107.0...v0.20170107.1)

- Add `getProjectStatusBadge`, `getProjectBranchStatusBadge`, and `getPublicProjectStatusBadge` operations for getting project build status badge images.
- Remove security for operations which do not require authentication.

## [v0.20170107.0](https://github.com/kevinoid/appveyor-swagger/tree/v0.20170107.0) (2017-01-13)


\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*
