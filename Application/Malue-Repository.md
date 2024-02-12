# Malue Asset Repository

The 'Malue Repository' is the container for all digital assets that are stored for use in Malue. Any type of digital asset can be stored in the Repository, for example:
- 	Pictures (jpeg, .png, .svg, .tiff, etc. )
- 	Video (.avi, .mp4, etc. )
- 	YouTube
- 	Documents (Word, PDF, etc. )

The repository is responsible for storing and indexing the assets so that they can be searched and retrieved in the most efficient manner. 

The repository could be implemented in Microsoft SharePoint, but many of our potential customers will not have licences and these would be prohibitively expensive to purchase simply to store documents. Rather we will implement an interface to an opens source CMS (Squidex at implementation) with the ability to re-implement on another CMS  or document storage platform if necessary. I think we should resist this, however, and make our own decisions on the best underlying architecture to use. 

Some medium to long term features may be:
	• Using GPT-4 (for example) AI tools to automatically summarise any documents
	• Deep contextual text search
	• Automated tagging and indexing of assets so that they are easily discovered
	• etc.

We're looking for a sort of **Notion** for Malue.