## Simple web phonebook application

The AWS CloudFormation Template in this project will launch an Amazon EC2 instance of type t2.micro with latest Amazon Linux 2 OS, bootstrap Apache/PHP, and install a simple address book web application. The template will also create an Amazon RDS MySQL database instance in free tier, i.e. of type db.t2.micro and with no Multi-AZ setup or read replicas. The WebTier Security Group will allow only SSH and HTTP connections to the web server (EC2 instance), and the DBTier Security Group will only allow the WebTier Security Group to initiate database connections to the RDS DB instance over the TCP port 3306.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

