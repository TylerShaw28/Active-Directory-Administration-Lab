# Active Directory Domain Administration and User Management Lab

## Project Overview

This project demonstrates hands-on experience configuring and administering an Active Directory environment using Windows Server 2022 and Windows 11 virtual machines in Oracle VirtualBox.

The objective of this lab was to gain practical experience with Active Directory Domain Services (AD DS), including creating organizational units, managing domain user accounts, configuring security groups, joining a Windows 11 workstation to a domain, and verifying domain authentication.

This lab simulates common IT administration tasks performed by Help Desk Technicians, IT Support Specialists, and System Administrators in business environments.

## Technologies Used
- Windows Server 2022
- Windows 11
- Oracle VirtualBox
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers (ADUC)

**Domain Name:** LAB.local

## Lab Objectives
- Create and organize Active Directory Organizational Units (OUs).
- Create and configure domain user accounts.
- Create departmental security groups.
- Join a Windows 11 workstation to an Active Directory domain.
- Verify successful computer registration within Active Directory.
- Test domain user authentication and password-change requirements.

### Step 1: Create an Organizational Unit for User Accounts

Using Active Directory Users and Computers (ADUC) on Windows Server 2022, I created a new Organizational Unit (OU) named Accounts within the LAB.local domain.

The purpose of this OU was to provide a centralized location for organizing and managing domain user accounts. I also enabled protection against accidental deletion to prevent unintended removal of the organizational unit.

<img width="951" height="916" alt="Create OU" src="https://github.com/user-attachments/assets/58f0f4fd-e2c4-4bc7-b6f6-4f1d80a81e74" />


*Figure 1: Creation of the Accounts Organizational Unit within the LAB.local domain.*

### Step 2: Create an Organizational Unit for Security Groups

I created a second Organizational Unit named Groups within the LAB.local domain using Active Directory Users and Computers.

This OU was established to separate departmental security groups from individual user accounts, improving the organization and administration of Active Directory objects. Protection against accidental deletion was also enabled.

<img width="949" height="909" alt="Create OU 2" src="https://github.com/user-attachments/assets/5964da66-99a7-4cd6-9d7c-adc2c21a10c3" />


*Figure 2: Creation of the Groups Organizational Unit for departmental security group management.*

### Step 3: Create Domain User Accounts

Using Active Directory Users and Computers, I created domain user accounts within the Accounts Organizational Unit.

During account configuration, I assigned an initial password and enabled the requirement for users to change their password at their next login.

This configuration demonstrates basic user account provisioning and password security practices commonly performed by IT administrators.

<img width="962" height="902" alt="Create User Jim Watkins" src="https://github.com/user-attachments/assets/d00fe4ba-9367-4d0c-a5b9-e13879ce279b" />


*Figure 3: Configuration of a domain user account with the requirement to change the password at next login.*

### Step 4: Verify Domain User Accounts

After creating the user accounts, I navigated to the Accounts Organizational Unit to verify that the accounts were successfully created.

I confirmed that the accounts for Jim Watkins and Patricia Johnson appeared within the designated OU.

This verification demonstrated that the domain accounts were created and organized correctly in Active Directory.

<img width="959" height="915" alt="Users" src="https://github.com/user-attachments/assets/6ced4c8b-a5c9-4855-85f4-4c81dd18a51d" />


*Figure 4: Verification of the Jim Watkins and Patricia Johnson user accounts within the Accounts Organizational Unit.*

### Step 5: Create Departmental Security Groups

Using Active Directory Users and Computers, I created two departmental security groups named Finance and HR within the Groups Organizational Unit.

These groups were created to establish a foundation for centralized access management and departmental organization.

In a business environment, security groups can be used to simplify permission management by allowing administrators to assign access rights to groups rather than individual users.

<img width="956" height="916" alt="Groups" src="https://github.com/user-attachments/assets/d5cbaff2-a916-43bd-a0aa-1c715432bcfb" />


*Figure 5: Finance and HR security groups created within the Groups Organizational Unit.*

### Step 6: Join a Windows 11 Workstation to the Domain

On the Windows 11 virtual machine, I accessed System Properties and changed the computer's membership from a workgroup to the LAB.local Active Directory domain.

After entering the required domain credentials, Windows displayed a confirmation message indicating that the workstation had successfully joined the domain.

Joining a computer to an Active Directory domain allows centralized user authentication and provides a foundation for managing workstations in an organizational environment.

<img width="959" height="912" alt="Added Windows 11 to Domain" src="https://github.com/user-attachments/assets/14e29284-4e2d-433c-a539-19c832c8e9f9" />


*Figure 6: Confirmation message displaying successful Windows 11 membership in the LAB.local domain.*

### Step 7: Verify Computer Registration in Active Directory

After successfully joining the Windows 11 workstation to the domain, I returned to Active Directory Users and Computers on Windows Server 2022.

I navigated to the Computers container within LAB.local and verified that the workstation named WINDOW11 appeared as a registered computer object.

This confirmed that the Windows 11 virtual machine had been successfully added to the Active Directory environment.

<img width="961" height="923" alt="Successfully Added Computer to Domain" src="https://github.com/user-attachments/assets/4d893430-cadd-4084-afcf-d539ffaf14d3" />


*Figure 7: Verification of the WINDOW11 computer account within the Active Directory Computers container.*

### Step 8: Test Domain Authentication and Password Change

To test domain authentication, I attempted to sign in to the Windows 11 workstation using the domain user account pjohnson.

During the sign-in process, Windows prompted the user to create and confirm a new password.

This demonstrated that the password-change requirement configured during account creation was being enforced when the user attempted to authenticate.

This step highlights how Active Directory supports centralized user authentication and password management across domain-joined computers.

<img width="964" height="851" alt="New User Change Password" src="https://github.com/user-attachments/assets/976eaedd-a390-4958-8b7f-4b9c3f1b5090" />


*Figure 8: Windows 11 sign-in displaying the mandatory password-change prompt for the pjohnson domain account.*

## Skills Demonstrated
- Active Directory Domain Services (AD DS)
- Windows Server 2022 Administration
- Active Directory Users and Computers (ADUC)
- Organizational Unit (OU) Management
- Domain User Account Creation
- Security Group Configuration
- Windows 11 Domain Joining
- Computer Account Verification
- Domain Authentication
- Password Management
- Oracle VirtualBox Virtualization
  
## Project Conclusion

Through this lab, I gained practical experience administering an Active Directory environment using Windows Server 2022 and Windows 11.

I successfully created and organized user accounts and security groups, configured Organizational Units, joined a Windows 11 workstation to the LAB.local domain, and verified computer registration and domain password-change enforcement.

This project strengthened my understanding of centralized identity management, domain administration, and Windows Server technologies commonly used in professional IT support environments.

The skills developed through this project are directly applicable to entry-level Help Desk, Desktop Support, and IT Support Specialist positions.
