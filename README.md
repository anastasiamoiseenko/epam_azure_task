{\rtf1\ansi\ansicpg1251\cocoartf2580
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fnil\fcharset0 Cambria;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;\red36\green64\blue132;\red24\green40\blue80;
}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;\cssrgb\c18431\c32941\c58824;\cssrgb\c12157\c21569\c38824;
}
{\*\listtable{\list\listtemplateid1\listhybrid{\listlevel\levelnfc0\levelnfcn0\leveljc0\leveljcn0\levelfollow0\levelstartat1\levelspace360\levelindent0{\*\levelmarker \{decimal\}.}{\leveltext\leveltemplateid1\'02\'00.;}{\levelnumbers\'01;}\fi-360\li720\lin720 }{\listname ;}\listid1}
{\list\listtemplateid2\listhybrid{\listlevel\levelnfc0\levelnfcn0\leveljc0\leveljcn0\levelfollow0\levelstartat1\levelspace360\levelindent0{\*\levelmarker \{decimal\}.}{\leveltext\leveltemplateid101\'02\'00.;}{\levelnumbers\'01;}\fi-360\li720\lin720 }{\listname ;}\listid2}
{\list\listtemplateid3\listhybrid{\listlevel\levelnfc0\levelnfcn0\leveljc0\leveljcn0\levelfollow0\levelstartat1\levelspace360\levelindent0{\*\levelmarker \{decimal\}.}{\leveltext\leveltemplateid201\'02\'00.;}{\levelnumbers\'01;}\fi-360\li720\lin720 }{\listname ;}\listid3}
{\list\listtemplateid4\listhybrid{\listlevel\levelnfc0\levelnfcn0\leveljc0\leveljcn0\levelfollow0\levelstartat6\levelspace360\levelindent0{\*\levelmarker \{decimal\}.}{\leveltext\leveltemplateid301\'02\'00.;}{\levelnumbers\'01;}\fi-360\li720\lin720 }{\listname ;}\listid4}
{\list\listtemplateid5\listhybrid{\listlevel\levelnfc0\levelnfcn0\leveljc0\leveljcn0\levelfollow0\levelstartat1\levelspace360\levelindent0{\*\levelmarker \{decimal\}.}{\leveltext\leveltemplateid401\'02\'00.;}{\levelnumbers\'01;}\fi-360\li720\lin720 }{\listname ;}\listid5}
{\list\listtemplateid6\listhybrid{\listlevel\levelnfc0\levelnfcn0\leveljc0\leveljcn0\levelfollow0\levelstartat1\levelspace360\levelindent0{\*\levelmarker \{decimal\}.}{\leveltext\leveltemplateid501\'02\'00.;}{\levelnumbers\'01;}\fi-360\li720\lin720 }{\listname ;}\listid6}}
{\*\listoverridetable{\listoverride\listid1\listoverridecount0\ls1}{\listoverride\listid2\listoverridecount0\ls2}{\listoverride\listid3\listoverridecount0\ls3}{\listoverride\listid4\listoverridecount0\ls4}{\listoverride\listid5\listoverridecount0\ls5}{\listoverride\listid6\listoverridecount0\ls6}}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\deftab720
\pard\pardeftab720\partightenfactor0

\f0\fs22 \cf2 ## Azure home task for EPAM DevOps course\
\pard\pardeftab720\sa40\partightenfactor0
\cf2 \
\pard\pardeftab720\sl259\slmult1\partightenfactor0

\fs26 \cf3 ### Part 1 \'96 Configure application\
\pard\tx360\tx720\pardeftab720\li720\fi-720\sl259\slmult1\sa160\partightenfactor0
\ls1\ilvl0
\fs22 \cf2 {\listtext	1.	}Create a service connection in a Azure DevOps project to your subscription\
\pard\pardeftab720\sl259\slmult1\sa160\partightenfactor0
\cf2 ![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_4_service_connecton.png\
2.  Find a pet project for the experiments\
I have chosen the simple node.js app to practice following after lectures\
3. Build your app locally (npm install/run build/run start)\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_3_run_locally.png\
4. Create an Azure DevOps repo\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_5_create_a_repo.png\
5. Create a branching policy for you application. Added yourself as a reviewer\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_6_dev_branch.png\
\pard\pardeftab720\sl259\slmult1\sa40\partightenfactor0

\fs26 \cf3 ### Part 2 \'96 Configure a pipeline to deploy infrastructure\
\pard\pardeftab720\sl259\slmult1\partightenfactor0

\fs24 \cf4 Terraform storage account \
\pard\tx360\tx720\pardeftab720\li720\fi-720\sl259\slmult1\sa160\partightenfactor0
\ls2\ilvl0
\fs22 \cf2 {\listtext	1.	}Create a separate resource group and deploy azure storage account\
\pard\pardeftab720\sl259\slmult1\sa160\partightenfactor0
\cf2 ![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_7_rg_and_storage_account.png\
2. Create a container with the name \'93tfstate\'94 and remember the name. use portal settings\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_8_tfstate_container.png\
\pard\pardeftab720\sl259\slmult1\partightenfactor0

\fs24 \cf4 #### Terraform preparation\
\pard\tx360\tx720\pardeftab720\li720\fi-720\sl259\slmult1\sa160\partightenfactor0
\ls3\ilvl0
\fs22 \cf2 {\listtext	1.	}Create another repo to store devops code\
{\listtext	2.	}Create a folder terraform\
{\listtext	3.	}Add app service implementation\
{\listtext	4.	}Integrate application insights with app service\
{\listtext	5.	}Updated backend \'93azurerm\'94 according to the guide\
\pard\pardeftab720\sl259\slmult1\sa160\partightenfactor0
\cf2 ![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_9_terraform.tf.png\
\pard\tx360\tx720\pardeftab720\li720\fi-720\sl259\slmult1\sa160\partightenfactor0
\ls4\ilvl0\cf2 {\listtext	6.	}Run az login or Connect-AzAccount to connect the azure subscription from your local\
{\listtext	7.	}Run terraform apply to deploy infrastructure \
\pard\pardeftab720\sl259\slmult1\sa160\partightenfactor0
\cf2 ![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_10_terraform_apply.png\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_11_terraform_apply_result.png\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_12_terraform_apply_result2.png\
\pard\pardeftab720\sl259\slmult1\partightenfactor0

\fs24 \cf4 #### Create a terraform pipeline\
\pard\tx360\tx720\pardeftab720\li720\fi-720\sl259\slmult1\sa160\partightenfactor0
\ls5\ilvl0
\fs22 \cf2 {\listtext	1.	}Create a yaml pipeline with the following steps: terraform install, terraform init, terraform plan/apply. Plan is an optional one \
{\listtext	2.	}Inside yaml pipeline add trigger to main branch. The scenario \'96 when main is updated, pipeline should run automatically\
{\listtext	3.	}Added 3 steps \'96 terraform install, terraform init, terraform plan/apply. Plan is an optional one. You may add it as 4
\fs14\fsmilli7333 \super th
\fs22 \nosupersub  step\
\pard\pardeftab720\sl259\slmult1\sa160\partightenfactor0
\cf2 ![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_13_terraform_pipeline.png\
![Image alt]({\field{\*\fldinst{HYPERLINK "https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_14_terraform_pipeline_result.png"}}{\fldrslt \ul https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_14_terraform_pipeline_result.png}}\
\pard\pardeftab720\partightenfactor0

\fs24 \cf2 ### Part 3 \'96 Create a deploy pipeline to app service\
\pard\pardeftab720\sl259\slmult1\sa160\partightenfactor0

\fs22 \cf2 \
\pard\tx360\tx720\pardeftab720\li720\fi-720\sl259\slmult1\sa160\partightenfactor0
\ls6\ilvl0\cf2 {\listtext	1.	}Add yml pipeline to the application folder\
{\listtext	2.	}Your pipeline structure should contain 2 stages. 1
\fs14\fsmilli7333 \super st
\fs22 \nosupersub  \'96 build, create zip archieve, and publish an artifact. 2
\fs14\fsmilli7333 \super nd
\fs22 \nosupersub  \'96 download an artifact and deploy it to azure app service\
\pard\pardeftab720\sl259\slmult1\sa160\partightenfactor0
\cf2 ![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_15_app_pipeline_result.png\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_16_app_pipeline_result.png\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_17_yaml1.png\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_18_yaml2.png\
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_19_yaml3.png}