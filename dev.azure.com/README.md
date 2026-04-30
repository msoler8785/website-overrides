# Azure DevOps - Custom CSS

This collection of CSS rules enhances the visual appearance and usability of various components within Azure DevOps. The styles provide a more compact layout for deployment group jobs and release pipeline lists, improve readability with font adjustments, and refine the overall interface for a cleaner, more efficient experience.

## Usage
Apply the styles using the following URL path: `https://dev.azure.com/*`

```css
// Compact view for deployment group jobs
.cd-logs-job-item {
	padding-top: 0.25rem !important;
	padding-bottom: 0.25rem !important;
	padding-left: 0.5rem !important;
	padding-right: 0.5rem !important;
}

.vertical-tab-item-description {
	display: flex;
	flex-direction: row;
	justify-content: space-between;
	width: 100%;
}

.vertical-tab-item-text.ellipsis-overflow {
	font-size: 0.75rem !important;
	font-weight: 600 !important;
}

// Use monospace font for textarea inputs.
.ms-TextField-field {
	font-family: 'Cascadia Code' !important;
}

// Compact view for release pipeline lists.
.act-rel-pipe-row {
	padding: 0;
}

.act-rel-pipe-row .flex-row {
	flex-direction: row-reverse;
}

.act-rel-pipe-row .row-content {
	display: flex;
	align-items: center;
	justify-content: space-between;
	margin-right: .5rem;
}

.act-rel-pipe-row .pipe-name {
	font-size: 0.875rem;
}

.active-rd-subtext {
	padding: 0;
}

.active-rd-subtext .pending-subtext {
	margin-right: 0.625rem;
}

.active-pipelines-table .bolt-button:hover {
	background-color: inherit;
}