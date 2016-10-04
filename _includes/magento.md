<p>Usage:</p>
<p>command [options] [arguments]</p>

<p>Options</p>
<table>
	<tbody>
		<tr>
			<td>--help (-h)</td><td>Displays help message</td>
		</tr>
		<tr>
			<td>--quiet (-q)</td><td>Do not output any message</td>
		</tr>
		<tr>
			<td>--verbose (-v|vv|vvv)</td><td>Increase the verbosity of messages: 1 for normal output, 2 for more verbose output and 3 for debug</td>
		</tr>
		<tr>
			<td>--version (-V)</td><td>Display this application version</td>
		</tr>
		<tr>
			<td>--ansi</td><td>Force ANSI output</td>
		</tr>
		<tr>
			<td>--no-ansi</td><td>Disable ANSI output</td>
		</tr>
		<tr>
			<td>--no-interaction (-n)</td><td>Do not ask any interactive question</td>
		</tr>
	</tbody>
</table>

<h3>Available commands</h3>
<table>
	<tbody>
		<tr>
			<td>help</td><td>Displays help for a command</td>
		</tr>
		<tr>
			<td>list</td><td>Lists commands</td>
		</tr>
	</tbody>
</table>
<h3>Admin</h3>
<table>
	<tbody>
		<tr>
			<td>admin:user:create</td><td>Creates an administrator</td>
		</tr>
		<tr>
			<td>admin:user:unlock</td><td>Unlock admin account</td>
		</tr>
	</tbody>
</table>
<h3>Cache</h3>
<table>
	<tbody>
		<tr>
			<td>cache:clean</td><td>Cleans cache type(s)</td>
		</tr>
		<tr>
			<td>cache:disable</td><td>Disables cache type(s)</td>
		</tr>
		<tr>
			<td>cache:enable</td><td>Enables cache type(s)</td>
		</tr>
		<tr>
			<td>cache:flush</td><td>Flushes cache storage used by cache type(s)</td>
		</tr>
		<tr>
			<td>cache:status</td><td>Checks cache status</td>
		</tr>
	</tbody>
</table>
<h3>Catalog</h3>
<table>
	<tbody>
		<tr>
			<td>catalog:images:resize</td><td>Creates resized product images</td>
		</tr>
	</tbody>
</table>
<h3>Cron</h3>
<table>
	<tbody>
		<tr>
			<td>cron:run</td><td>Runs jobs by schedule</td>
		</tr>
	</tbody>
</table>
<h3>Customer</h3>
<table>
	<tbody>
		<tr>
			<td>customer:hash:upgrade</td><td>Upgrade customer's hash according to the latest algorithm</td>
		</tr>
	</tbody>
</table>
<h3>Deploy</h3>
<table>
	<tbody>
		<tr>
			<td>deploy:mode:set</td><td>Set application mode</td>
		</tr>
		<tr>
			<td>deploy:mode:show</td><td>Displays current application mode</td>
		</tr>
	</tbody>
</table>
<h3>Dev</h3>
<table>
	<tbody>
		<tr>
			<td>dev:source-theme:deploy</td><td>Collects and publishes source files for theme</td>
		</tr>
		<tr>
			<td>dev:tests:run</td><td>Runs tests</td>
		</tr>
		<tr>
			<td>dev:urn-catalog:generate</td><td>Generates the catalog of URNS to *.xsd</td>
		</tr>
		<tr>
			<td>dev:xml:convert</td><td>Converts XML file using XSL style sheets</td>
		</tr>
	</tbody>
</table>
<h3>i18n</h3>
<table>
	<tbody>
		<tr>
			<td>i18n:collect-phrases</td><td>Discovers phrases in the codebase</td>
		</tr>
		<tr>
			<td>i8n:pack</td><td>Saves language package</td>
		</tr>
		<tr>
			<td>i18n:uninstall</td><td>Uninstalls language packages</td>
		</tr>
	</tbody>
</table>
<h3>Indexer</h3>
<table>
	<tbody>
		<tr>
			<td>indexer:info</td><td>Shows allowed indexers</td>
		</tr>
		<tr>
			<td>indexer:reindex</td><td>Reindexes data</td>
		</tr>
		<tr>
			<td>indexer:set-mode</td><td>Sets index mode type</td>
		</tr>
		<tr>
			<td>indexer:show-mode</td><td>Shows index mode</td>
		</tr>
		<tr>
			<td>indexer:status</td><td>Shows status of indexer</td>
		</tr>
	</tbody>
</table>
<h3>Maintenance</h3>
<table>
	<tbody>
		<tr>
			<td>maintenance:allow-ips</td><td>Sets maintenance mode exempt IPs</td>
		</tr>
		<tr>
			<td>maintenance:disable</td><td>Disables maintenance mode</td>
		</tr>
		<tr>
			<td>maintenance:enable</td><td>Enables maintenance mode</td>
		</tr>
		<tr>
			<td>maintenance:status</td><td>Displays maintenance mode status</td>
		</tr>
	</tbody>
</table>
<h3>Module</h3>
<table>
	<tbody>
		<tr>
			<td>module:disable</td><td>Disables specified modules</td>
		</tr>
		<tr>
			<td>module:enable</td><td>Enables specified modules</td>
		</tr>
		<tr>
			<td>module:status</td><td>Displays status of modules</td>
		</tr>
		<tr>
			<td>module:uninstall</td><td>Uninstalls modules installed by composer</td>
		</tr>
	</tbody>
</table>
<h3>Sampledata</h3>
<table>
	<tbody>
		<tr>
			<td>sampledata:deploy</td><td>Deploy sample data modules</td>
		</tr>
		<tr>
			<td>sampledata:remove</td><td>Remove all sample data from composer.json</td>
		</tr>
		<tr>
			<td>sampledata:reset</td><td>Reset sample data modules for re-installation</td>
		</tr>
	</tbody>
</table>
<h3>Theme</h3>
<table>
	<tbody>
		<tr>
			<td>theme:uninstall</td><td>Uninstalls theme</td>
		</tr>
	</tbody>
</table>
<h3>Info</h3>
<table>
	<tbody>
		<tr>
			<td>info:adminuri</td><td>Displays the Magento Admin URI</td>
		</tr>
		<tr>
			<td>info:backups:list</td><td>Prints list of available backup files</td>
		</tr>
		<tr>
			<td>info:currency:list</td><td>Displays the list of available currencies</td>
		</tr>
		<tr>
			<td>info:dependencies:show-framework</td><td>Shows number of dependencies on Magento framework</td>
		</tr>
		<tr>
			<td>info:dependencies:show-modules</td><td>Shows number of dependencies between modules</td>
		</tr>
		<tr>
			<td>info:dependencies:show-modules-circular</td><td>Shows number of circular dependencies between modules</td>
		</tr>
		<tr>
			<td>info:language:list</td><td>Displays the list of available language locales</td>
		</tr>
		<tr>
			<td>info:timezone:list</td><td>Displays the list of available timezones</td>
		</tr>
	</tbody>
</table>
<h3>Setup</h3>
<table>
	<tbody>
		<tr>
			<td>setup:backup</td><td>Takes backup of Magento Application code base, media and database</td>
		</tr>
		<tr>
			<td>setup:config:set</td><td>Creates or modifies the deployment configuration</td>
		</tr>
		<tr>
			<td>setup:cron:run</td><td>Runs cron job scheduled for setup application</td>
		</tr>
		<tr>
			<td>setup:db-data:upgrade</td><td>Installs and upgrades data in the DB</td>
		</tr>
		<tr>
			<td>setup:db-schema:upgrade</td><td>Installs and upgrades the DB schema</td>
		</tr>
		<tr>
			<td>setup:db:status</td><td>Checks if the DB schema or data requires upgrade</td>
		</tr>
		<tr>
			<td>setup:di:compile</td><td>Generates DI configuration and all non-existing interceptors and factories</td>
		</tr>
		<tr>
			<td>setup:di:compile-multi-tenant</td><td>Generates all non-existing proxies and factories, and pre-compile class definitions, inheritance information and plugin definitions</td>
		</tr>
		<tr>
			<td>setup:install</td><td>Installs the Magento application</td>
		</tr>
		<tr>
			<td>setup:performance:generate-fixtures</td><td>Generates fixtures</td>
		</tr>
		<tr>
			<td>setup:rollback</td><td>Rolls back Magento Application codebase, media and database</td>
		</tr>
		<tr>
			<td>setup:static-content:deploy</td><td>Deploys static view files</td>
		</tr>
		<tr>
			<td>setup:store-config:set</td><td>Installs the store configuration</td>
		</tr>
		<tr>
			<td>setup:uninstall</td><td>Uninstalls the Magento application</td>
		</tr>
		<tr>
			<td>setup:upgrade</td><td>Upgrades the Magento application, DB data, and schema</td>
		</tr>
	</tbody>
</table>
