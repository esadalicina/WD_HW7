REST APIs assignment:

Below you can see the documentation of the .js file, which already describes the API methods.
There are 4 different methods post, get, put and delete.
post: This method create a city
get: With get you can have the city information
put: With put you can update the population value
delete: Here you can delete a specific city with all his values

With this documentation you can get the API website but there need to be add some things extra, which was done in the last assignment.

/**
 * @api {post} /test1 Create new city
 * @apiGroup DB_City
 * @apiName GetNewCity
 * @apiParam {String} Name City name
 * @apiParam {String} CountryCode City country code
 * @apiParam {String} District City district
 * @apiParam {Number} Population City population number
 * @apiParamExample {json} Input
 *    {
 *      "Name": "Bissen",
 *      "CountryCode": "LUX",
 *      "District": "Mersch",
 *      "Population": 432
 *    }
 * @apiSuccess {String} message Success message
 * @apiSuccessExample {json} Success
 *    HTTP/1.1 200 OK
 *    {
 *      "message": "Successfully created"
 *    }
 * @apiError {String} message Error message
 * @apiErrorExample {json} List error
 *    HTTP/1.1 500 Internal Server Error
 *    {
 *      "message": "Creation failed"
 *    }
*/

/**
 * @api {get} /test2 Get city info
 * @apiGroup DB_City
 * @apiName GetCity
 * @apiParam {String} Name City Name
 * @apiSuccess {Number} id City id
 * @apiSuccess {String} name City name
 * @apiSuccess {String} countryCode City countryCode
 * @apiSuccess {String} district City district
 * @apiSuccess {Number} population City population number
 * @apiSuccessExample {json} Success
 *    HTTP/1.1 200 OK
 *    {
 *      "id": 25,
 *      "name": "Haarlemmermeer",
 *      "countryCode": "NLD",
 *      "district": "Noord-Holland",
 *      "population": 110722
 *    }
 * @apiErrorExample {json} List error
 *    HTTP/1.1 500 Internal Server Error
 */
 
 /**
 * @api {put} /test3 Update population number
 * @apiGroup DB_City
 * @apiName UpdatePopulation
 * @apiParam {String} Name City name
 * @apiParam {Number} Population City population number
 * @apiParamExample {json} Input
 *    {
 *      "Name": "Bissen",
 *      "Population": 500
 *    }
 * @apiSuccess {Number} id City id
 * @apiSuccess {String} name City name
 * @apiSuccess {String} countryCode City countryCode
 * @apiSuccess {String} district City district
 * @apiSuccess {Number} population City population number
 * @apiSuccessExample {json} Success
 *    HTTP/1.1 200 OK
 *    {
 *      "id": 4080,
 *      "name": "Bissen",
 *      "countryCode": "LUX",
 *      "district": "Mersch",
 *      "population": 500
 *    }
 * @apiErrorExample {json} List error
 *    HTTP/1.1 500 Internal Server Error
*/

/**
 * @api {delete} /test4 Delete city
 * @apiGroup DB_City
 * @apiName DeleteCity
 * @apiParam {String} Namen City name
 * @apiParamExample {json} Input
 *    {
 *      "Name": "Bissen"
 *    }
 * @apiSuccess {String} message Success message
 * @apiSuccessExample {json} Success
 *    HTTP/1.1 200 OK
 *    {
 *      "message": "true"
 *    }
 * @apiError {String} message Error message
 * @apiErrorExample {json} List error
 *    HTTP/1.1 500 Internal Server Error
 *    {
 *      "message": "false"
 *    }
*/