# Resource-principal-Object-storage-access-from-functions
Connect and read from Object storage from within an oracle function using resource principal authentication.

• Following Function guideline to set up function. https://docs.cloud.oracle.com/en-us/iaas/Content/Functions/Concepts/functionsprerequisites.htm

• Create Function Application: https://docs.cloud.oracle.com/en-us/iaas/Content/Functions/Tasks/functionscreatingapps.htm

Create dynamic group including the function. Create policy to give nosql access for dynakuc group in compartment or tenancy.

Notes: If seeing function timeout, update func.yaml to increase. Fn: Error invoking function. status: 504 message: Timed out

Add "timeout: 120" to func.yaml
