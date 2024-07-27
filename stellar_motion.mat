% starData is a dataset containg the information needed for the project
% Was provided by default in the MATLAB Onramp
% Code is seperated into blocks, run them individually within an IDE

load starData
nObs = size(spectra,1)
lambdaStart = 630.02
lambdaDelta = 0.14

lambdaEnd = lambdaStart + (nObs-1)*lambdaDelta
lambda = (lambdaStart:lambdaDelta:lambdaEnd)

s = spectra(:,2)

plot(lambda,s,".-")
xlabel("Wavelength")
ylabel("Intensity")

[sHa,idx] = min(s)
lambdaHa = lambda(idx)

hold on
plot(lambdaHa,sHa,"rs",MarkerSize=8)
hold off

z = lambdaHa/656.28 - 1
speed = z*299792.458
