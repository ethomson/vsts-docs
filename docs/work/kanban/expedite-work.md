---
title: Use swimlanes to expedite work | VSTS & TFS
description: Use swimlanes to differentiate different types of work you track on the Kanban board in Visual Studio Team Services (VSTS) and Team Foundation Server (TFS)
ms.technology: vs-devops-wit
ms.prod: vs-devops-alm
ms.assetid: 0BBD90C3-7156-4027-B100-9E46F5BD53FB
ms.manager: douge
ms.author: kaelli
ms.date: 10/20/2017
---

# Expedite work

<b>VSTS | TFS 2018 | TFS 2017 | TFS 2015</b> 

Your Kanban board supports your ability to visualize the flow of work as it moves from new to done. When you add swimlanes, you can also visualize the status of work that supports different service-level classes. You can create a swimlane to represent any other dimension that supports your tracking needs.    

For example, you can create three swimlanes&mdash;Expedite, Standard, and Park&mdash;to track high-priority work, standard work, and work that's currently blocked.  

<img src="_img/ALM_EW_IntroChart_3C.png" alt="Kanban board showing three swimlanes" style="border: 2px solid #C3C3C3;" /> 

>[!TIP]
>Type <span style="color:purple; font-family:Courier new; font-size:1.1em; font-weight:bold">o</span> to expand all swimlanes and <span style="color:purple; font-family:Courier new; font-size:1.1em; font-weight:bold">u</span> to collapse all swimlanes. To move the focus up or down, enter the ![Up/Down arrow](../_img/icons/Arrow_Up.png)![ ](../_img/icons/Arrow_Down.png) up/down arrows. For more tips, see [Keyboard shortcuts](../../collaborate/keyboard-shortcuts.md).


## Types of swimlanes  
You can use swimlanes to sort work on your Kanban board to track items that you differentiate as follows: 
*	High priority items  
*	Service-level class  
*	Date-driven requirement  
*	Dependency for or from another team   
*	Blocked items  
*	Technical debt or other engineering work that's not a specific user story  


## Track work in swimlanes  
Once you've set up your swimlanes, you can drag items into a swimlane as well as reorder them within the lane.  

<img src="_img/ALM_EW_MoveToNewLane.png" alt="Kanban board, Drag items into a swimlane" style="border: 2px solid #C3C3C3;" /> 

You can also focus on a single swimlane by collapsing all other lanes.

<img src="_img/ALM_EW_CollapseLanes.png" alt="Kanban board, Collapsed swimlanes" style="border: 2px solid #C3C3C3;" />  

## Configure swimlanes 
So, what swimlanes will support your tracking needs?  

Once you've identified one or two, add them to your working Kanban board.  

1. From your Kanban board, click ![settings icon](../_img/icons/team-settings-gear-icon.png) and as needed, click Swimlanes.  

	<img src="../customize/_img/kanban-card-customize-open-settings.png" alt="Kanban board, open common configuration settings" style="border: 2px solid #C3C3C3;" /> 

	If you're not a team admin, [get added as one](../scale/add-team-administrator.md). Only team and project admins can customize the Kanban board.

2.	Click ![add icon](../_img/icons/add_icon.png) and enter the name of the swimlane you want to add.  
	
	**VSTS and TFS 2015.1:**  

	<img src="_img/kanban-board-add-swimlane.png" alt="Kanban board, Add a swimlane" style="border: 2px solid #C3C3C3;" />    

	The default lane appears unlabeled on the Kanban board. You can rename it to anything you like, however, you can't delete it. Also, you can rename it directly from the Kanban board. 

	**TFS 2015:**   

	![Add a swimlane](_img/ALM_SW.AddLane.png)  

	The default lane is automatically renamed to Standard when you add a second lane. You can rename it to anything you like, however, you can't delete it. 

3.	To reorder your swimlanes, simply grab the lane and move it up or down.

	<img src="_img/ALM_EW_ReorderLanes.png" alt="Kanban board, Open swimlanes" style="border: 2px solid #C3C3C3;" />

4.	If you need to delete a lane, first move all items out of the lane, and then click Delete from the lane's context menu.  

	<img src="_img/ALM_EW_DeleteLane.png" alt="Kanban board, Delete a swimlane" style="border: 2px solid #C3C3C3;" />

## Related Kanban notes

As you can see, swimlanes provides another way to organize and visualize the flow of work using [Kanban](kanban-basics.md). Here are a few more options you have for customizing the look and feel of your Kanban board.   

*	[Add columns](add-columns.md)  
*	[Work in Progress limits](wip-limits.md)   
*	[Split columns](split-columns.md)   
*	[Definition of Done](definition-of-done.md)   
*	[Customize cards](../customize/customize-cards.md)   
*	[Show bugs on backlogs and boards](../customize/show-bugs-on-backlog.md)   

### Tracking lane moves  


**VSTS and TFS 2015.1 and later versions**

You can track Kanban board swimlane moves using the [Board Lane field](../track/query-by-workflow-changes.md#kanban_query_fields).  

**TFS 2015**

Similar to the way [column moves are tracked](add-columns.md), swimlane moves are captured in the history field.  

<img src="_img/ALM_EW_HistorySwimLanes.png" alt="Work item form, History tab, History of a swimlane move" style="border: 2px solid #C3C3C3;" />   

For TFS 2015 and earlier versions, you can't [query](../track/using-queries.md) for all items in a particular swimlane. To perform such a query, you'd have to assign a value to a field, such as the Priority field, or [tag](../track/add-tags-to-work-items.md) each item in a similar way.  

###REST API resources
To programmatically interact with Kanban board and other team settings, see the [Work API reference](https://www.visualstudio.com/en-us/integrate/api/work/overview).
