5 steps to RBAC

What is Role Based Access Control (RBAC) and why do we care?
"RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role."

Describe a Role/Permission heirarchy that you might implement using RBAC.
Admin vs. Manager, Instructors vs Students, IT vs. Admin, etc.

What approach might you take to implement RBAC?

1. inventory systems
2. analyze your workfroce and create roles
3. assign people to roles 
4. never make one-off changes
5. audit 

wiki - RBAC

If Authentication is “you are who you say you are,” what is Authorization? Authentication verifies that you are who you say you are while authorization determines what permissions you have and what you have access to.

Name three primary rules defined for RBAC.
  1. Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.
  2. Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
  3. Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.

Describe RBAC to a non-technical friend.
  It is the approach of allowing people different permissions/access based on their role within an organization.

RBAC tutorial

What Are access rights Associated with? The User? or The Role? Explain.

  Rights are associated with the role you have
  Users must first be associated with a role before having any rights


Access Rights, or Authorization, is activated after a user successfully does what? Is assigned a role

Explain how RBAC might benefit a business.
  Policies don't need to be updated when a person in a specific role leaves the company

  New employees can then just access their assigned roles

  Accessibility controls for what the role specifically needs 
Reflection
What are your learning goals after reading and reviewing the class README?

sources:
https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html
https://en.wikipedia.org/wiki/Role-based_access_control
https://www.youtube.com/watch?v=C4NP8Eon3cA
