# DCPPC RFC Implementation Process (DRAFT)

-----------
## DCPPC Request for Comment (RFC) Instructions and Guidelines


1. Read the [background document to the DCPPC-RFC process](#background).  Your group’s DCPPC-RFC should align with the principles and roles therein.
2. Create a written draft your DCPPC-RFC as a Google Doc and set the Google Doc Sharing Status as "Anyone with the link can comment"
	a. The location of the DCPPC-RFC document folder will be provided by DCPPC project management staff
3. Except for the header, the format of the DCPPC-RFC Google Doc is not prescriptive and should contain content sufficient for the DCPPC-RFC-Type (defined next) and any supporting information or other documents.   The DCPPC-RFC header placed at the beginning of the DCPPC-RFC should contain this information:
	* DCPPC-RFC-# {NOTE: Leave blank as this will be assigned by DCPPC-RFC-Governance in Step 4 upon initial submission}
	* DCPPC-RFC-Title
	* DCPPC-RFC-Version (starting with 1, incremented as required by DCPPC-RFC-Governance in Step 7)
	* DCPPC-RFC-Type (click the type for definition):
		* [Standards](#standards)
		* [Process](#process)
		* [Consensus Building](#consensus-building)
		* [Informational](#informational)
	* Name of the person who is to be Point of Contact for the RFC
	* Email of the person who is to be Point of Contact for the RFC
	* Submitting Group (e.g. KC#)
	* Requested RFC posting start date
	* Requested RFC posting end date
	* Date Emailed for consideration
	* DCPPC-RFC-Status : (DCPPC-RFC-Governance will assign an initial value of “Active and open RFC period” updating with values in Steps 6 and 8 as required)
	* URL Link to GitHub : (DCPPC-RFC-Governance will assign a link of where intermediate and final PDFs are stored per Step 9)
	* URL Link to Google Doc : (URL of DCPPC-RFC Google Doc for a given RFC)

4. Email the RFC Google Doc URL to DCPPC-RFC-Governance {Owen, Titus, Stan}
	a. Within 1 business day, they will either approve and post to {leads@dcppc.groups.io, nih-dcppc general slack channel} or email back Point of Contact requesting refinement or clarification
	b. If posted to {leads@dcppc.groups.io, nih-dcppc general slack channel}, a unique DCPPC-RFC tag will be assigned based on the pattern: 
DCPPC-RFC-#  where # is an assigned sequential number 
5. Once an approved DCPPC-RFC-# posted to {leads@dcppc.groups.io, nih-dcppc general slack channel}	, the NIH Data Commons community will be proactively encouraged to comment on it during the requested posting period.
	a. DCPPC project management staff will broadly announce the DCPPC RFC on the start date, halfway through the suggested duration, the day prior, and on the RFC end date.
	b. Cross-posting by by any NIH DCPPC development participants is encouraged.
6. Upon conclusion of the DCPPC-RFC-# posting period, the Submitting Group will have ten business days to address comments provided in the DCPPC-RFC-#, assign one of the follow DCPPC-RFC-Status values, and email to DCPPC-RFC-Governance:
	a. Propose-Resolved
	b. Propose-Merge (i.e. with another RFC)
	c. Propose-Postpone
	d.Propose-Unsuccessful
	e. Propose-Withdrawn
7. DCPPC-RFC-Governance will either agree or disagree with the DCPPC-RFC-Status assigned value of the Submitting Group in Step 6:
	a. If DCPPC-RFC-Governance agrees with the DCPPC-RFC-Status value assigned by the Submitting Group , then the modified DCPPC-RFC-# will be posted for a Final Comment Period (FCP) of no less than 5 business days.
	b. If DCPPC-RFC-Governance disagrees with the DCPPC-RFC-Status value assigned by the Submitting Group , DCPPC-RFC-Governance will assign a different DCPPC-RFC-Status from the list in Step 6 along with a written explanation and email back to the Point of Contact to restart the DCPPC-RFC process at Step 3 incrementing DCPPC-RFC-Version by 1, or at their discretion, proceed to Step 8 without further iteration.
8. Upon conclusion of the DCPPC-RFC-# Final Comment Period (FCP) or at their discretion, the DCPPC-RFC-Governance will assign one of the following DCPPC-RFC-Status values concluding the DCPPC-RFC process without further iteration:
	a. Resolved
	b. Merged (i.e. with another RFC)
	c. Postponed
	d. Unsuccessful
	e. Withdrawn
9. All versions of of a given DCPPC-RFC Google Doc will be named will be named with Google version history, and an individual PDF of each named version including all contributor comments therein associated with that version will be placed in https://github.com/dcppc/internal/rfcs. 







## DCPPC-RFC-Types
#### Standards
A **Standards** Track DCPPC-RFC describes a new feature or implementation for the NIH Data Commons. It may also describe an interoperability standard that will be supported across the full stacks. Candidate specification must be implemented and tested for correct operation and interoperability by multiple independent parties and utilized in increasingly demanding environments, before it can be adopted as an DCPPC Standard. Candidate specifications should include a description of any external standards that were considered, used, adapted, or rejected.

#### Process
A **Process** DCPPC-RFC describes a process surrounding the NIH Data Commons, or proposes a change to (or an event in) a process. Process DCPPC-RFCs are like Standards Track DCPPC-RFCs but apply to areas other than the NIH Data Commons code itself. They may propose an implementation, but not to NIH Data Commons codebase.  Unlike Informational DCPPC-RFCs, they are more than recommendations, and users are typically not free to ignore them. Examples include procedures, guidelines, and changes to the decision-making process. 

#### Consensus Building
A **Consensus Building** DCPPC-RFC describes a NIH Data Commons design issue, or provides general guidelines or information to the NIH Data Commons development community, and may propose a new feature. Unlike Informational DCPPC-RFCs, Consensus Building DCPPC-RFC represent a NIH Data Commons community consensus or recommendation, so users and implementers are expected to make a best effort to follow their advice.

#### Informational
An **Informational** DCPPC-RFC describes a NIH Data Commons design issue, or provides general guidelines or information to the NIH Data Commons development community, but does not propose a new feature. Informational DCPPC-RFCs do not necessarily represent a NIH Data Commons community consensus or recommendation, so users and implementers are free to ignore Informational DCPPC-RFCs or follow their advice.






## Background on DCPPC-RFCs
#### Background
The activities of both the Full Stacks (FSs) and the Key Capabilities (KCs) play a vital role in the Data Commons (DC), and are also critical to the NHLBI Data STAGE. In the process of building the Data Commons we must make decisions, but we need to make decisions based on feedback from individual contributors, the FSs, the KCs, and the many NIH stakeholders, including Data STAGE.  Further, there is considerable overlap and interaction between the KCs and the FSs, but they have somewhat different responsibilities and timelines.  As a result, we need to establish a process that enables effective interactions between the KCs and the FSs, and also supports shared decision making.  To accomplish this, we propose the use of Requests for Comments (RFCs).

Principles that support the need for RFCs:
1. Where possible, we enable individual contributors and teams to independently make the decisions necessary to build components, to build the FSs, and to subsequently build the DC.
2. We actively seek feedback from a broad community of domain experts, and not all of those experts are part of the teams building the KCs, the FSs, the DC, or STAGE.
3. The KCs provide domain expertise and also build communities-of-practice.
4. The KCs help the DC to manage the risk in building the DC.
5. The KCs are responsible for not only providing feedback on the current technology, but also provide context and feedback on future technologies.
6. The KCs operate asynchronously from the FSs.
7. The FSs will seek input from a broad community of stakeholders outside the DCPPC.
8. By using RFCs the work of building the DC can proceed as multiple, interoperable and  parallel projects, thus permitting exploration and resiliency.

The KCs’ roles are:
1. Each KC focuses on challenges that fall within an area of competence that must be addressed for the DC, and as such they act as community conveners to encourage exploration and innovation.
2. In cases when challenges and solutions overlap or have dependencies with other KCs, the KC will involve other KCs and divide the discussions and responsibilities appropriately. 
3. They act as working groups that evaluate key areas of technology necessary for the Data Commons (DC).
4. The KCs may implement products that are  intended to be used by the FSs on an ongoing basis.
5. The KCs put forward Requests for RFCs to solicit feedback on key areas in which standards may need to emerge.

The FSs’ roles are:
1. Each FS focuses on a set of challenges that must be addressed for a particular implementation of the DC, as well as the interoperability of the components they build across other stacks.
2. The FSs act as development teams that implement and evaluate key areas of technology necessary for the Data Commons.
3. The FSs put forward RFCs to solicit feedback on key areas in which standards may need to emerge.

An RFC should include participation from all the FS teams. Interaction between KCs and FSs
1. The KCs serve as the group that provides in-depth technical analysis of possible choices for a given DC challenge and will implement resources to be used by the FS where necessary.
2. The FSs serve as the primary implementers of capabilities that are eventually deployed. As such the FSs depend on and are informed by the technical analysis done the KCs.
3. Sharing of KC analyses across the multiple teams allows cross-fertilization of options and approaches across the FSs.

Using the RFC process, through consultation with the broader community, allows the KCs and the FSs to:
1. Initiate or refine potential standards, or 
2. Establish or improve a DCPPC process, or
3. Build consensus among competing technologies, or
4. Provide broadly useful information.

Generally, an RFC should be created when:
1. We seek to reach agreement.
2. We seek to establish a contract between actors.
3. We are defining conventions, e.g.,  interfaces, APIs, data models, etc.
4. There is a need for transparency and inclusion on a necessary decision.
5. A decision could impact more than one system component or team or stakeholders.
6. We are adding dependencies that can affect more than one team.


Sources: https://opensource.com/article/17/9/6-lessons-rfcs; https://www.python.org/dev/peps/pep-0001/; https://opensource.com/business/12/6/architecture-participation; https://en.wikipedia.org/wiki/Request_for_Comments; http://aturon.github.io/2018/05/25/listening-part-1/

