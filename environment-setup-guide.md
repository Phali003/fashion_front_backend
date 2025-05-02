# Setting Up Environment Variables in Vercel Dashboard

## Step 1: Access Your Project's Environment Variables

1. Navigate to https://vercel.com/phalis-projects-56e327f7/food-ecommerce/settings/environment-variables
2. You'll need to be logged in to your Vercel account
3. You should see the Environment Variables page that looks like this:

![Vercel Environment Variables Page](https://i.imgur.com/example1.png)

## Step 2: Add the Required Environment Variables

Click "Add New" and add each of these variables one by one:

| Name | Value | Environment |
|------|-------|-------------|
| NODE_ENV | production | Production |
| JWT_SECRET | p8e4t92URzt2QmMBxZxRX9k6VPwN3Dcp2jGf3sK5vM4 | Production |
| JWT_EXPIRES_IN | 24h | Production |
| COOKIE_SECRET | bK9yD7mX4vR2nL8pQ5sW9cF3hJ6tN4mV2xP7dC8k | Production |
| COOKIE_SECURE | true | Production |
| COOKIE_HTTP_ONLY | true | Production |
| COOKIE_SAME_SITE | strict | Production |
| COOKIE_MAX_AGE | 86400000 | Production |

For each variable:
1. Enter the name (e.g., NODE_ENV)
2. Enter the value (e.g., production)
3. Select "Production" environment
4. Click "Add"

## Step 3: Verify the Variables Were Added

After adding all variables, your page should display them in the list. They will appear as hidden values for security reasons.

## Step 4: Redeploy Your Application

After adding the environment variables:

1. Go to the Deployments tab in your Vercel project
2. Find your latest deployment
3. Click the three dots menu (⋮) next to it
4. Select "Redeploy" to apply the new environment variables

## Next Steps: Database Setup

Once you've added the environment variables and redeployed your application, we can proceed with:

1. Setting up a cloud database (MySQL on Railway, PlanetScale, or another provider)
2. Configuring the database connection
3. Testing the full application functionality

Let me know when you've completed these steps or if you need further assistance with any part of the process.

