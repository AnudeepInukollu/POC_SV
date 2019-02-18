Solar Village
=======================

Below steps briefly describes the End to End process that was developed as part of this POC:

1) The Process starts with the inputs "Order Id" & "Customer Type" from the user.

2) The provided inputs can be validated by a clerk through clerk task and accept or reject the application accordingly.(Clerk will approve only "Resident" or "HOAMember".

3) Based on the Customer Type, the applications can be routed for the different approvals. 

4) Customer Type should be "Resident" to skip approval of House owner Association. "HOAMember" should go through sales offier acknowledgement & HOA approval.

5) For the Human tasks, sales offier acknowledgement & HOA approval, they can approve by clicking the checkbox available. Completing the task without checking the box can be termed as a rejection. If a sales officer didnot accept the invitation, then the task can be reassigned automatically to the group again. Rejection from HOA Ends the Process.


6) Created Mock data from Work Item Handlers for mocking Structural & Residential Approvals based on Order Id.

7) Pre-defined Mock data : 

	orderId = 1 ; Rejects both approvals
	orderId = 2 ; Approve Structural & Reject Residential
	orderId = 3 ; Approve Residential & Reject Structural 
	Rest all OrderId ; Approve both

8) If one of the permit is approved and the other is rejected, the approved permit will be rescind through WIH.

