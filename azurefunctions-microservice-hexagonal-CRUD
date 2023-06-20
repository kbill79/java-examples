import com.microsoft.azure.functions.annotation.*;
import com.microsoft.azure.functions.*;

public class Function {
    @FunctionName("create")
    public HttpResponseMessage create(
            @HttpTrigger(name = "req", methods = {HttpMethod.POST}, authLevel = AuthorizationLevel.ANONYMOUS) HttpRequestMessage<Optional<String>> request,
            final ExecutionContext context) {
        context.getLogger().info("Java HTTP trigger processed a request.");

        // Parse request body
        String requestBody = request.getBody().orElse(null);
        if (requestBody == null) {
            return request.createResponseBuilder(HttpStatus.BAD_REQUEST).body("Please pass a name in the request body").build();
        }

        // TODO: Implement create logic

        return request.createResponseBuilder(HttpStatus.OK).body("Created").build();
    }

    @FunctionName("read")
    public HttpResponseMessage read(
            @HttpTrigger(name = "req", methods = {HttpMethod.GET}, authLevel = AuthorizationLevel.ANONYMOUS) HttpRequestMessage<Optional<String>> request,
            final ExecutionContext context) {
        context.getLogger().info("Java HTTP trigger processed a request.");

        // TODO: Implement read logic

        return request.createResponseBuilder(HttpStatus.OK).body("Read").build();
    }

    @FunctionName("update")
    public HttpResponseMessage update(
            @HttpTrigger(name = "req", methods = {HttpMethod.PUT}, authLevel = AuthorizationLevel.ANONYMOUS) HttpRequestMessage<Optional<String>> request,
            final ExecutionContext context) {
        context.getLogger().info("Java HTTP trigger processed a request.");

        // Parse request body
        String requestBody = request.getBody().orElse(null);
        if (requestBody == null) {
            return request.createResponseBuilder(HttpStatus.BAD_REQUEST).body("Please pass a name in the request body").build();
        }

        // TODO: Implement update logic

        return request.createResponseBuilder(HttpStatus.OK).body("Updated").build();
    }

    @FunctionName("delete")
    public HttpResponseMessage delete(
            @HttpTrigger(name = "req", methods = {HttpMethod.DELETE}, authLevel = AuthorizationLevel.ANONYMOUS) HttpRequestMessage<Optional<String>> request,
            final ExecutionContext context) {
        context.getLogger().info("Java HTTP trigger processed a request.");

        // TODO: Implement delete logic

        return request.createResponseBuilder(HttpStatus.OK).body("Deleted").build();
    }
}
