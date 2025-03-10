## API Report File for "@backstage/plugin-catalog"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
/// <reference types="react" />

import { AddLocationRequest } from '@backstage/catalog-client';
import { AddLocationResponse } from '@backstage/catalog-client';
import { ApiHolder } from '@backstage/core-plugin-api';
import { BackstagePlugin } from '@backstage/core-plugin-api';
import { CatalogApi } from '@backstage/catalog-client';
import { CatalogClient } from '@backstage/catalog-client';
import { CatalogRequestOptions } from '@backstage/catalog-client';
import { Entity } from '@backstage/catalog-model';
import { EntityName } from '@backstage/catalog-model';
import { ExternalRouteRef } from '@backstage/core-plugin-api';
import { GetEntitiesRequest } from '@backstage/catalog-client';
import { GetEntitiesResponse } from '@backstage/catalog-client';
import { GetEntityAncestorsRequest } from '@backstage/catalog-client';
import { GetEntityAncestorsResponse } from '@backstage/catalog-client';
import { IconComponent } from '@backstage/core-plugin-api';
import { IdentityApi } from '@backstage/core-plugin-api';
import { InfoCardVariants } from '@backstage/core-components';
import { Location as Location_2 } from '@backstage/catalog-model';
import { Overrides } from '@material-ui/core/styles/overrides';
import { PropsWithChildren } from 'react';
import { default as React_2 } from 'react';
import { ReactNode } from 'react';
import { RouteRef } from '@backstage/core-plugin-api';
import { StyleRules } from '@material-ui/core/styles/withStyles';
import { TableColumn } from '@backstage/core-components';
import { TableProps } from '@backstage/core-components';
import { TabProps } from '@material-ui/core';
import { UserListFilterKind } from '@backstage/plugin-catalog-react';

// Warning: (ae-forgotten-export) The symbol "AboutCardProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-missing-release-tag) "AboutCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function AboutCard({ variant }: AboutCardProps): JSX.Element;

// Warning: (ae-forgotten-export) The symbol "Props" needs to be exported by the entry point index.d.ts
// Warning: (ae-missing-release-tag) "AboutContent" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const AboutContent: ({ entity }: Props) => JSX.Element;

// Warning: (ae-forgotten-export) The symbol "Props" needs to be exported by the entry point index.d.ts
// Warning: (ae-missing-release-tag) "AboutField" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const AboutField: ({
  label,
  value,
  gridSizes,
  children,
}: Props_2) => JSX.Element;

// @public (undocumented)
export type BackstageOverrides = Overrides & {
  [Name in keyof PluginCatalogComponentsNameToClassKey]?: Partial<
    StyleRules<PluginCatalogComponentsNameToClassKey[Name]>
  >;
};

// Warning: (ae-missing-release-tag) "CatalogClientWrapper" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public @deprecated
export class CatalogClientWrapper implements CatalogApi {
  constructor(options: { client: CatalogClient; identityApi: IdentityApi });
  // (undocumented)
  addLocation(
    request: AddLocationRequest,
    options?: CatalogRequestOptions,
  ): Promise<AddLocationResponse>;
  // (undocumented)
  getEntities(
    request?: GetEntitiesRequest,
    options?: CatalogRequestOptions,
  ): Promise<GetEntitiesResponse>;
  // (undocumented)
  getEntityAncestors(
    request: GetEntityAncestorsRequest,
    options?: CatalogRequestOptions,
  ): Promise<GetEntityAncestorsResponse>;
  // (undocumented)
  getEntityByName(
    compoundName: EntityName,
    options?: CatalogRequestOptions,
  ): Promise<Entity | undefined>;
  // (undocumented)
  getLocationByEntity(
    entity: Entity,
    options?: CatalogRequestOptions,
  ): Promise<Location_2 | undefined>;
  // (undocumented)
  getLocationById(
    id: string,
    options?: CatalogRequestOptions,
  ): Promise<Location_2 | undefined>;
  // (undocumented)
  getOriginLocationByEntity(
    entity: Entity,
    options?: CatalogRequestOptions,
  ): Promise<Location_2 | undefined>;
  // (undocumented)
  refreshEntity(
    entityRef: string,
    options?: CatalogRequestOptions,
  ): Promise<void>;
  // (undocumented)
  removeEntityByUid(
    uid: string,
    options?: CatalogRequestOptions,
  ): Promise<void>;
  // (undocumented)
  removeLocationById(
    id: string,
    options?: CatalogRequestOptions,
  ): Promise<void>;
}

// Warning: (ae-missing-release-tag) "CatalogEntityPage" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const CatalogEntityPage: () => JSX.Element;

// Warning: (ae-missing-release-tag) "CatalogIndexPage" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const CatalogIndexPage: (props: DefaultCatalogPageProps) => JSX.Element;

// Warning: (ae-forgotten-export) The symbol "CatalogKindHeaderProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-missing-release-tag) "CatalogKindHeader" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const CatalogKindHeader: ({
  initialFilter,
}: CatalogKindHeaderProps) => JSX.Element;

// Warning: (ae-missing-release-tag) "catalogPlugin" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
const catalogPlugin: BackstagePlugin<
  {
    catalogIndex: RouteRef<undefined>;
    catalogEntity: RouteRef<{
      name: string;
      kind: string;
      namespace: string;
    }>;
  },
  {
    createComponent: ExternalRouteRef<undefined, true>;
    viewTechDoc: ExternalRouteRef<
      {
        name: string;
        kind: string;
        namespace: string;
      },
      true
    >;
  }
>;
export { catalogPlugin };
export { catalogPlugin as plugin };

// Warning: (ae-missing-release-tag) "CatalogResultListItem" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const CatalogResultListItem: ({ result }: any) => JSX.Element;

// Warning: (ae-missing-release-tag) "CatalogTable" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const CatalogTable: {
  ({ columns, actions }: CatalogTableProps): JSX.Element;
  columns: typeof columnFactories;
};

// Warning: (ae-missing-release-tag) "EntityRow" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export type CatalogTableRow = {
  entity: Entity;
  resolved: {
    name: string;
    partOfSystemRelationTitle?: string;
    partOfSystemRelations: EntityName[];
    ownedByRelationsTitle?: string;
    ownedByRelations: EntityName[];
  };
};

// Warning: (ae-missing-release-tag) "createMetadataDescriptionColumn" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function createMetadataDescriptionColumn(): TableColumn<CatalogTableRow>;

// Warning: (ae-forgotten-export) The symbol "NameColumnProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-missing-release-tag) "createNameColumn" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function createNameColumn(
  props?: NameColumnProps,
): TableColumn<CatalogTableRow>;

// Warning: (ae-missing-release-tag) "createOwnerColumn" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function createOwnerColumn(): TableColumn<CatalogTableRow>;

// Warning: (ae-missing-release-tag) "createSpecLifecycleColumn" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function createSpecLifecycleColumn(): TableColumn<CatalogTableRow>;

// Warning: (ae-missing-release-tag) "createSpecTypeColumn" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function createSpecTypeColumn(): TableColumn<CatalogTableRow>;

// Warning: (ae-missing-release-tag) "createSystemColumn" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function createSystemColumn(): TableColumn<CatalogTableRow>;

// Warning: (ae-missing-release-tag) "createTagsColumn" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function createTagsColumn(): TableColumn<CatalogTableRow>;

// @public
export type DefaultCatalogPageProps = {
  initiallySelectedFilter?: UserListFilterKind;
  columns?: TableColumn<CatalogTableRow>[];
  actions?: TableProps<CatalogTableRow>['actions'];
};

// Warning: (ae-missing-release-tag) "EntityAboutCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityAboutCard: AboutCard;

// Warning: (ae-missing-release-tag) "EntityDependencyOfComponentsCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityDependencyOfComponentsCard: ({
  variant,
  title,
}: {
  variant?: 'gridItem' | undefined;
  title?: string | undefined;
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityDependsOnComponentsCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityDependsOnComponentsCard: ({
  variant,
  title,
}: {
  variant?: 'gridItem' | undefined;
  title?: string | undefined;
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityDependsOnResourcesCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityDependsOnResourcesCard: ({
  variant,
}: {
  variant?: 'gridItem' | undefined;
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityHasComponentsCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityHasComponentsCard: ({
  variant,
}: {
  variant?: 'gridItem' | undefined;
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityHasResourcesCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityHasResourcesCard: ({
  variant,
}: {
  variant?: 'gridItem' | undefined;
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityHasSubcomponentsCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityHasSubcomponentsCard: ({
  variant,
}: {
  variant?: 'gridItem' | undefined;
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityHasSystemsCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityHasSystemsCard: ({
  variant,
}: {
  variant?: 'gridItem' | undefined;
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityLayout" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public
export const EntityLayout: {
  ({
    UNSTABLE_extraContextMenuItems,
    UNSTABLE_contextMenuOptions,
    children,
  }: EntityLayoutProps): JSX.Element;
  Route: (props: SubRoute) => null;
};

// Warning: (ae-missing-release-tag) "EntityLinksCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityLinksCard: ({
  cols,
  variant,
}: {
  entity?: Entity | undefined;
  cols?: number | ColumnBreakpoints | undefined;
  variant?: 'gridItem' | undefined;
}) => JSX.Element;

// @public (undocumented)
export type EntityLinksEmptyStateClassKey = 'code';

// Warning: (ae-missing-release-tag) "EntityListContainer" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntityListContainer: ({
  children,
}: PropsWithChildren<{}>) => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityOrphanWarning" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public
export const EntityOrphanWarning: () => JSX.Element;

// Warning: (ae-missing-release-tag) "EntityPageLayout" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public @deprecated
export const EntityPageLayout: {
  ({
    children,
    UNSTABLE_extraContextMenuItems,
    UNSTABLE_contextMenuOptions,
  }: EntityPageLayoutProps): JSX.Element;
  Content: (_props: {
    path: string;
    title: string;
    element: JSX.Element;
  }) => null;
};

// Warning: (ae-missing-release-tag) "EntityProcessingErrorsPanel" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public
export const EntityProcessingErrorsPanel: () => JSX.Element | null;

// Warning: (ae-missing-release-tag) "EntitySwitch" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const EntitySwitch: {
  ({ children }: PropsWithChildren<{}>): JSX.Element | null;
  Case: (_: {
    if?:
      | ((
          entity: Entity,
          context: {
            apis: ApiHolder;
          },
        ) => boolean | Promise<boolean>)
      | undefined;
    children: ReactNode;
  }) => null;
};

// Warning: (ae-missing-release-tag) "FilterContainer" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const FilterContainer: ({
  children,
}: PropsWithChildren<{}>) => JSX.Element;

// Warning: (ae-missing-release-tag) "FilteredEntityLayout" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const FilteredEntityLayout: ({
  children,
}: PropsWithChildren<{}>) => JSX.Element;

// Warning: (ae-missing-release-tag) "hasCatalogProcessingErrors" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const hasCatalogProcessingErrors: (
  entity: Entity,
  context: {
    apis: ApiHolder;
  },
) => Promise<boolean>;

// Warning: (ae-missing-release-tag) "isComponentType" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function isComponentType(type: string): (entity: Entity) => boolean;

// Warning: (ae-missing-release-tag) "isKind" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function isKind(kind: string): (entity: Entity) => boolean;

// Warning: (ae-missing-release-tag) "isNamespace" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export function isNamespace(namespace: string): (entity: Entity) => boolean;

// Warning: (ae-missing-release-tag) "isOrphan" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const isOrphan: (entity: Entity) => boolean;

// @public (undocumented)
export type PluginCatalogComponentsNameToClassKey = {
  PluginCatalogEntityLinksEmptyState: EntityLinksEmptyStateClassKey;
  PluginCatalogSystemDiagramCard: SystemDiagramCardClassKey;
};

// Warning: (ae-missing-release-tag) "RelatedEntitiesCard" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public (undocumented)
export const RelatedEntitiesCard: <T extends Entity>(props: {
  variant?: 'gridItem' | undefined;
  title: string;
  columns: TableColumn<T>[];
  entityKind?: string | undefined;
  relationType: string;
  emptyMessage: string;
  emptyHelpLink: string;
  asRenderableEntities: (entities: Entity[]) => T[];
}) => JSX.Element;

// Warning: (ae-missing-release-tag) "Router" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public @deprecated (undocumented)
export const Router: ({
  EntityPage,
}: {
  EntityPage?: React_2.ComponentType<{}> | undefined;
}) => JSX.Element;

// @public (undocumented)
export type SystemDiagramCardClassKey =
  | 'domainNode'
  | 'systemNode'
  | 'componentNode'
  | 'apiNode'
  | 'resourceNode';

// Warnings were encountered during analysis:
//
// src/components/CatalogTable/CatalogTable.d.ts:10:5 - (ae-forgotten-export) The symbol "CatalogTableProps" needs to be exported by the entry point index.d.ts
// src/components/CatalogTable/CatalogTable.d.ts:11:5 - (ae-forgotten-export) The symbol "columnFactories" needs to be exported by the entry point index.d.ts
// src/components/EntityLayout/EntityLayout.d.ts:43:5 - (ae-forgotten-export) The symbol "EntityLayoutProps" needs to be exported by the entry point index.d.ts
// src/components/EntityLayout/EntityLayout.d.ts:44:5 - (ae-forgotten-export) The symbol "SubRoute" needs to be exported by the entry point index.d.ts
// src/components/EntityPageLayout/EntityPageLayout.d.ts:22:5 - (ae-forgotten-export) The symbol "EntityPageLayoutProps" needs to be exported by the entry point index.d.ts
// src/plugin.d.ts:22:5 - (ae-forgotten-export) The symbol "ColumnBreakpoints" needs to be exported by the entry point index.d.ts
```
