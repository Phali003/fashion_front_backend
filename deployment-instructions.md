# Vercel Deployment Instructions for Fashion Front-Backend

Your application has been successfully deployed to Vercel at:
https://vercel.com/phalis-projects-56e327f7/fashion-front-backend

## Setting Up Environment Variables

To make your application function correctly, you need to add these environment variables in your Vercel dashboard:

1. Go to https://vercel.com/phalis-projects-56e327f7/fashion-front-backend
2. Click on "Settings" at the top navigation
3. Select "Environment Variables" from the left sidebar
4. Add the following variables:

```
NODE_ENV=production
JWT_SECRET=p8e4t92URzt2QmMBxZxRX9k6VPwN3Dcp2jGf3sK5vM4
JWT_EXPIRES_IN=24h
COOKIE_SECRET=bK9yD7mX4vR2nL8pQ5sW9cF3hJ6tN4mV2xP7dC8k
COOKIE_SECURE=true
COOKIE_HTTP_ONLY=true
COOKIE_SAME_SITE=strict
COOKIE_MAX_AGE=86400000
```

5. Make sure to select "Production" for the environment
6. Click "Save" after adding all variables
7. Vercel will automatically redeploy your application with the new environment variables

## Managing Your Deployment

You can use these Vercel CLI commands to manage your deployment:

```
# View deployment logs
npx vercel logs fashion-front-backend

# View build details
npx vercel inspect fashion-front-backend

# Redeploy after making changes to your code
npx vercel --prod
```

## Next Steps

1. Verify that your frontend is working correctly by visiting your deployment URL
2. Set up a cloud database (MySQL on Railway, PlanetScale, etc.) for your backend
3. Add the database connection details to your Vercel environment variables:
   ```
   DATABASE_URL=your_database_connection_string
   ```
4. Test the full application functionality including database operations

